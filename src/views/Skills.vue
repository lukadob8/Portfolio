<template>
    <div>
        <h1>My Tech Stack</h1>
        <img src="../assets/skills.jpg" alt="Photo of some code." width="200px">
        <br><br>
        <menu-bar />
        <h3>I have experience with the following technologies:</h3>
        <div>
            <div id="stack">
                <p>HTML5</p>
                <p>CSS/SCSS</p>
                <p>JavaScript</p>
                <p>Vue.js</p>
                <p>Python</p>
                <p>Flask</p>
                <p>SQL</p>
            </div>
            <p>In addition to those mentioned above I have experience deploying live sites using the Google Cloud and apache2. As well as using github for version control.</p>
        </div>
    </div>
</template>

<script>
import MenuBar from "../components/menu.vue";

    export default {
        name: "skills-page",
        components: {
            MenuBar,
        },
    }
</script>

<style scoped>
img{
    border-radius: 50%;
    
}
#stack {
    display: grid;
    grid-template-columns: 1fr 1fr;
}
</style>