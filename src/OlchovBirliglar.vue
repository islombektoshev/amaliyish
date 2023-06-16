<template>
  <div id="app/olchov_birliglar">
    <h1>O'lchov Birliglar</h1>
    <label for="app/olchov_birliglar/a">Sonni kriting</label><br>
    <input type="number" id="app/olchov_birliglar/a" placeholder="a = " v-model="a"><br>
    <table>
      <tr>
        <td>{{ a }} <span>Tonna</span></td>
        <td> =</td>
        <td>{{ a * 1000 }} <span>Kilogram</span></td>
      </tr>
      <tr>
        <td>{{ a }} <span>Kilogram</span></td>
        <td> =</td>
        <td>{{ a / 1000 }} <span>Tonna</span></td>
      </tr>
      <tr>
        <td>{{ a }} <span>Kilogram</span></td>
        <td> =</td>
        <td>{{ a * 1000 }} <span>Gram</span></td>
      </tr>
      <tr>
        <td>{{ a }} <span>Gram</span></td>
        <td> =</td>
        <td>{{ a / 1000 }} <span>Kilogram</span></td>
      </tr>
    </table>
    <br>
  </div>
</template>
<script>
export default {
  name: 'OlchovBirliglar',
  data: () => ({a: 0})
}
</script>
<style>

* {
  background-color: white; /* rgba(255, 0,0,5%); */
  outline: none;
}

</style>