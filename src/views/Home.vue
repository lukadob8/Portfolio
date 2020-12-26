<template>
  <div class="home">
    <div id="intro">
      <div id="title">
        <h1>Hi my name is Luka</h1>
        <h4>I am a recent Full Stack Web Developer graduate looking to improve my skills!</h4>
      </div>
    </div>
   <menu-bar />
   <div id="about">

   </div>
  </div>
</template>

<script>
import MenuBar from "../components/menu.vue"
// @ is an alias to /src


export default {
  name: "Home",
  components: {
    MenuBar,
  },
  data() {
    return {
      
    }
  },
};
</script>

<style scoped>

</style>