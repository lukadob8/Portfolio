<template>
  <div class="home">
    <div id="intro">
      <div id="title">
        <h1>Luka Dobrijevic</h1>
        <img src="../assets/luka.jpg" alt="Profile image for portfolio site." width="200px" />
        <h4>Jr Full Stack Web Developer</h4>
      </div>
    </div>
    <menu-bar />
    <div id="about">
      <div>
        <h2>About</h2>
      </div>
      <div>
        <p>Hi, my name is Luka. I am a recent graduate from the Full Stack Web Development Diploma from InnoTech College. Prior to beginning my studies in web dev I worked in marketing and advertising. I had many roles including: team lead, sales, geurilla marketing and event coordinating. I am excited to combine the skills I learned in these roles with my newfound knowledge and passion for web design.</p>
      </div>
      <div>
        <a href="https://drive.google.com/file/d/1FlA8f99KGrgMEzL39oHY_b3jUosZpXhp/view?usp=sharing"><p>Click Here to Download my Resume</p></a>
      </div>
    </div>
  </div>
</template>

<script>
import MenuBar from "../components/menu.vue";
// @ is an alias to /src

export default {
  name: "Home",
  components: {
    MenuBar
  },
  data() {
    return {};
  }
};
</script>

<style scoped>
img {
  border-radius: 50%;
}
#home {
  display: grid;
  
}
h2 {
  text-decoration: underline solid;
}
</style>