<template>
  <div>
    <div id="DTmenu">
      <button @click="toHome()">Home</button>
      <button @click="toProjects()">Projects</button>
      <button @click="toSkills()">Skills</button>
      <button @click="toContact()">Contact</button>
    </div>
    <div id="mobile-grid">
      <div id="Drop-menu">
        <input type="checkbox" name="mobile-menu-checkbox" id="mobile-menu-checkbox" />

        <div id="mobile-hamburger-container">
          <span id="mobile-line-1" class="mobile-hamburger-line"></span>
          <span id="mobile-line-2" class="mobile-hamburger-line"></span>
          <span id="mobile-line-3" class="mobile-hamburger-line"></span>
        </div>

        <div id="header-menu">
          <button @click="toHome()">Home</button>
          <button @click="toProjects()">Projects</button>
          <button @click="toSkills()">Skills</button>
          <button @click="toContact()">Contact</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "menu-bar",
  methods: {
    toProjects: function() {
      this.$router.push({ name: "Projects" });
    },

    toSkills: function() {
      this.$router.push({ name: "Skills" });
    },

    toContact: function() {
      this.$router.push({ name: "Contact" });
    },

    toHome: function() {
      this.$router.push({ name: "Home" });
    }
  }
};
</script>

<style scoped>
#mobile-grid {
  display: grid;
  width: 100%;
  min-height: 10vh;
  justify-items: center;
}

#mobile-menu-checkbox {
  width: 50px;
  height: 50px;
  position: absolute;
  opacity: 0;
  z-index: 5;
}

#mobile-menu-checkbox:checked ~ #header-menu {
  top: 0;
  opacity: 1;
  transition: all 0.5s ease-in-out;
}

#mobile-hamburger-container {
  display: grid;
  justify-items: center;
  align-items: center;
  width: 50px;
  height: 50px;
  z-index: 4;
  position: relative;
}

.mobile-hamburger-line {
  width: 30px;
  height: 4px;
  background-color: black;
}

#header-menu {
  transition: all 0.5s ease-in-out;
  position: absolute;
  width: 100%;
  background-color: lightblue;
  display: grid;
  justify-items: center;
  align-items: center;
  top: -60vh;
  opacity: 0;
  left: 0;
  min-height: 40vh;
}

#DTmenu {
  display: none;
}

@media only screen and (min-width: 600px) {
  html {
    font-size: 1.5em;
  }

  #Drop-menu {
    display: none;
  }

  #DTmenu {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr;
    column-gap: 50px;
  }
}
</style>