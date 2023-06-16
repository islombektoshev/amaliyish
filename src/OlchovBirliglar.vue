<template>
  <div id="app/olchov_birliglar" style="max-width: 400px">
    <h1>O'lchov Birliglar</h1>
    <label class="form-control"  for="app/olchov_birliglar/a">Sonni kriting</label>
    <input class="form-control" type="number" id="app/olchov_birliglar/a" placeholder="a = " v-model="a"><br>
    <table class="table">
      <tbody>
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
      </tbody>
    </table>
  </div>
</template>
<script>
export default {
  name: 'OlchovBirliglar',
  data: () => ({a: 0})
}
</script>
<style>

</style>