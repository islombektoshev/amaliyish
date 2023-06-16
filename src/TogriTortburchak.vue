<template>
  <div id="app/togri_tort_burchak">
    <h1>Tog'ri To'rt Burchak</h1>
    <img
        src="https://media.geeksforgeeks.org/wp-content/uploads/Rectangle-.jpg"
        width="300px"
        alt="Tog'ri to'rtbuchak">
    <br>
    <label for="app/butunsonlar/input/a">A ning qiymatini kiriting</label><br>
    <input type="number" id="app/butunsonlar/input/a" v-model="a" placeholder="a = "><br>
    <label for="app/butunsonlar/input/b">B ning qiymatini kiriting</label><br>
    <input type="number" id="app/butunsonlar/input/b" v-model="b" placeholder="b = "><br>

    <table>
      <tr>
        <td>Yuzasi</td>
        <td>{{ a * b }}</td>
      </tr>
      <tr>
        <td>Perimeter</td>
        <td>{{ 2*(parseFloat(a) + parseFloat(b)) }}</td>
      </tr>
    </table>


    <br>
  </div>
</template>
<script>
export default {
  name: 'TogriTortburchak',
  data: () => ({a: 0, b: 0})
}
</script>
<style>

* {
  background-color: white; /* rgba(255, 0,0,5%); */
  outline: none;
}

</style>