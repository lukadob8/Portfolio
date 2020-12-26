<template>
    <div>
        <div id="menu">
            <button>Projects</button>
            <button>Skills</button>
            <button>Contact</button>
        </div>
    </div>
</template>

<script>
    export default {
        name: "menu-bar",
        methods: {
            toProjects: function() {
                this.$router.push({name: "Projects"})
            },

            toSkills: function() {
                this.$router.push({name: "Skills"})
            },

            toContact: function() {
                this.$router.push({name: "Contact"})
            },
        },
    }
</script>

<style scoped>
#menu {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    column-gap: 50px;
}
</style>