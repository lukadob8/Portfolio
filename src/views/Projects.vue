<template>
    <div>
        <h1>My Projects</h1>
        <img src="../assets/projects.jpg" alt="A photo of some code.">
        <br><br>
        <menu-bar />
        <div id="projects">
            <div class="items">
                <h2>Okotoks Pizza</h2>
                <img src="../assets/okoPizza.png" alt="Home page of okopizza.">
                <p>This was my first ever project. The goal was to create a website for a fake local pizza restaurant.</p>
                <p>Tech stack: HTML, CSS/SCSS</p>
                <a href="https://okopizza.ml/" target="_blank">Live Site</a>
                <br>
                <a href="https://github.com/lukadob8/OkotoksPizzaProject.git" target="_blank">Git Hub</a>
                <br>
            </div>
            <div class="items">
                <h2>Tweeter</h2>
                <img src="../assets/tweeter.png" alt="Home page of tweeterfull.">
                <p>The second project I worked on was a clone of Twitter. The project was broken down into two parts. First the front end and then the back end. This is also the first full stack project I have made.</p>
                <p>Tech stack: Vue.js, Python, SQL, MariaDB</p>
                <a href="https://tweeterfull.ml/#/signup" target="_blank">Live Site</a>
                <br>
                <a href="https://github.com/lukadob8/VueTweeter.git" target="_blank">Frontend Git Hub</a>
                <br>
                <a href="https://github.com/lukadob8/tweeterBackend.git" target="_blank">Backend Git Hub</a>
                <br>
            </div>
            <div class="items">
                <h2>uQuery</h2>
                <img src="../assets/uQuery.png" alt="Home page of uQuery.">
                <p>For my final project I decided to make a full stack CRUD application. uQuery is a question and answer application where users have the ability to post questions, answer questions and vote on the best answers. It takes inspiration from Stack Overflow and Yahoo answers.</p>
                <p>Tech stack: Vue.js, Python, SQL, MariaDB</p>
                <a href="https://uquery.ml/#/" target="_blank">Live Site</a>
                <br>
                <a href="https://github.com/lukadob8/MVPFrontend.git" target="_blank">Frontend Git Hub</a>
                <br>
                <a href="https://github.com/lukadob8/MVPBackend.git" target="_blank">Backend Git Hub</a>
                <br>
            </div>

        </div>
    </div>
</template>

<script>
import MenuBar from "../components/menu.vue"

    export default {
        name: "projects-page",
        components: {
            MenuBar,
        },
    }
</script>

<style scoped>
img{
    width: 200px;
    border: solid;
    border-radius: 50%;
}
#projects {
    display: grid;
    align-items: center;
    justify-items: center;
    padding: 40px;
}
.items {
    display: grid;
    align-items: center;
    justify-items: center;
     border-bottom: solid;
}
</style>