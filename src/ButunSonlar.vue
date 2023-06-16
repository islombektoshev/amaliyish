<template>
  <div id="app/butunsonlar">
    <h1>Butun Sonlar Ustida Amallar</h1>
    <label for="app/butunsonlar/input/a">A ning qiymatini kiriting</label><br>
    <input type="number" id="app/butunsonlar/input/a" v-model="a" placeholder="a = "><br>
    <label for="app/butunsonlar/input/b">B ning qiymatini kiriting</label><br>
    <input type="number" id="app/butunsonlar/input/b" v-model="b" placeholder="b = "><br>
    <table>
      <tr><td>A - B = </td><td>{{parseFloat(a)-parseFloat(b)}}</td></tr>
      <tr><td>A + B = </td><td>{{parseFloat(a)+parseFloat(b)}}</td></tr>
      <tr><td>A * B = </td><td>{{parseFloat(a)*parseFloat(b)}}</td></tr>
      <tr><td>A / B = </td><td>{{ parseFloat(a) / parseFloat(b)}}</td></tr>
    </table>
  </div>
</template>
<script>
export default {
  name: 'ButunSonlar',
  data: ()=>({
    a:0,
    b:0
  })
}
</script>
<style>

* {
  background-color: white; /* rgba(255, 0,0,5%); */
  outline: none;
}

</style>