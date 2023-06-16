<template>
  <div id="app/butunsonlar" style="max-width: 400px">
    <h1>Butun Sonlar Ustida Amallar</h1>
    <label class="form-control" for="app/butunsonlar/input/a">A ning qiymatini kiriting</label>
    <input class="form-control" type="number" id="app/butunsonlar/input/a" v-model="a" placeholder="a = "><br>
    <label class="form-control" for="app/butunsonlar/input/b">B ning qiymatini kiriting</label>
    <input class="form-control" type="number" id="app/butunsonlar/input/b" v-model="b" placeholder="b = "><br>
    <table class="table">
      <tbody>
      <tr>
        <td>A - B</td>
        <td>{{ parseFloat(a) - parseFloat(b) }}</td>
      </tr>
      <tr>
        <td>A + B</td>
        <td>{{ parseFloat(a) + parseFloat(b) }}</td>
      </tr>
      <tr>
        <td>A * B</td>
        <td>{{ parseFloat(a) * parseFloat(b) }}</td>
      </tr>
      <tr>
        <td>A / B</td>
        <td>{{ parseFloat(a) / parseFloat(b) }}</td>
      </tr>

      </tbody>
    </table>

  </div>
</template>
<script>
export default {
  name: 'ButunSonlar',
  data: () => ({
    a: 0,
    b: 0
  })
}
</script>
<style>


</style>