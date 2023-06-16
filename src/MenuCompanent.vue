<template>
  <div style="display: flex; height: 100vh; flex-direction: column; justify-content: center; align-items: center">
    <div
        style="display: flex; flex-direction: column; width: 300px; height: 100px; align-items: start; justify-content: space-between">
      <h1>Arslonova Sultona <br>6-Sinf Matematika</h1>
      <div><input id="app/menu/radio/0" type="radio" v-model="menu" value="0"> <label for="app/menu/radio/0">Butun
        sonlar ustida ammalar</label></div>
      <div><input id="app/menu/radio/1" type="radio" v-model="menu" value="1"> <label for="app/menu/radio/1">O'lchov
        birliglari</label></div>
      <div><input id="app/menu/radio/2" type="radio" v-model="menu" value="2"> <label for="app/menu/radio/2">To'g'ri
        to'rtburchak</label></div>

      <button @click="buttonClick" style="align-self: end">keyingi</button>
    </div>

  </div>
</template>
<script>
export default {
  /* eslint-disable */
  name: 'MenuCompanent',
  data: () => ({
    menu: 0
  }),
  methods: {
    buttonClick(e) {
      this.$emit('menu', parseInt(this.menu))
    }
  }
}
</script>
<style>
* {
  background-color: rgba(100, 0, 0, 5%);
  outline: 1px solid black;
}

body {
  margin: 0;
}
</style>