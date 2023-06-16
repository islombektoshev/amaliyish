<template>
  <div id="app/togri_tort_burchak" style="max-width: 400px">
    <h1>Tog'ri To'rt Burchak</h1>
    <img
        src="https://media.geeksforgeeks.org/wp-content/uploads/Rectangle-.jpg"
        width="300px"
        alt="Tog'ri to'rtbuchak">
    <br>
    <label class="form-control" for="app/butunsonlar/input/a">A ning qiymatini kiriting</label>
    <input class="form-control" type="number" id="app/butunsonlar/input/a" v-model="a" placeholder="a = "><br>
    <label class="form-control" for="app/butunsonlar/input/b">B ning qiymatini kiriting</label>
    <input class="form-control" type="number" id="app/butunsonlar/input/b" v-model="b" placeholder="b = "><br>

    <table class="table">
      <tbody>
      <tr>
        <td>Yuzasi</td>
        <td>{{ a * b }}</td>
      </tr>
      <tr>
        <td>Perimeter</td>
        <td>{{ 2 * (parseFloat(a) + parseFloat(b)) }}</td>
      </tr>
      </tbody>
    </table>

  </div>
</template>
<script>
export default {
  name: 'TogriTortburchak',
  data: () => ({a: 0, b: 0})
}
</script>
<style>


</style>