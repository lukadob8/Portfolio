<template>
    <div>
        <div>
            <h1>Contact</h1>
            <img src="../assets/Contact2.jpg" alt="A photo of a phone." width="200px">
        </div>
        <br>
        <br>
        <menu-bar />
        <div id="info">
            <div>
            <h2>Email:</h2>
            <a href="mailto:lukad@telus.net">lukad@telus.net</a>
            </div>
            <div>
                <h2>Phone:</h2>
                <a id="mobile-phone" href="tel:7802935852">780-293-5852</a>
                <p id="dt-phone">780-293-5852</p>
            </div>
            <div>
                <h2>LinkedIn:</h2>
                <a href="https://www.linkedin.com/in/luka-dobrijevic-aa6546a5/"> <p>Click Here</p></a>
            </div>
            <div>
                <h2>Git Hub:</h2>
                <a href="https://github.com/lukadob8">Click Here</a>
            </div>
            <div>
                <h3>Interested in working together?</h3>
                <p>Please send me an email to the above address with your name, project requirements and contact info and I will reply as soon as possible!</p>
            </div>
        </div>
    </div>
</template>

<script>
import MenuBar from "../components/menu.vue"
    export default {
        components: {
            MenuBar,
        },
    }
</script>

<style scoped>
img{
    border: 0;
    border-radius: 100%;
}

#dt-phone {
    display: none;
}
</style>