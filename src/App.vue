<template>
  <MenuCompanent v-if="menu === -1" @menu="oneMenuChosen"/>
  <div v-else style="margin: 20px">
    <ButunSonlar v-if="menu === 0"/>
    <OlchovBirliglar v-if="menu === 1"/>
    <TogriTortburchak v-if="menu === 2"/>
    <button @click="() => {menu = -1}">Ortga</button>
  </div>

</template>

<script>
/* eslint-disable */
import MenuCompanent from "@/MenuCompanent.vue";
import ButunSonlar from "@/ButunSonlar.vue";
import OlchovBirliglar from "@/OlchovBirliglar.vue";
import TogriTortburchak from "@/TogriTortburchak.vue";

export default {
  name: 'App',
  data() {
    return {
      menu: -1
    }
  },
  methods: {
    oneMenuChosen(m) {
      this.menu = m;
      console.log(m)
    }
  },
  components: {
    TogriTortburchak,
    OlchovBirliglar,
    ButunSonlar,
    MenuCompanent

  }
}

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

* {
  background-color: white; /* rgba(255, 0,0,5%); */
  outline: none;
}

</style>
