<template>
    <div>
        <h1>My Projects</h1>
        <img src="../assets/projects.jpg" alt="A photo of some code.">
        <br><br>
        <menu-bar />
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
    border-radius: 50%;
}

</style>