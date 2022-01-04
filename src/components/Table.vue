<template>
    <table class="table">
  <thead>
    <tr>
      <th scope="col">ID</th>
      <th scope="col">Nombre</th>
      <th scope="col">Tipo</th>
      <th scope="col">Handle</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row" v-for="item in datos" :key="item.id">1</th>
      <td>{{item.id}}</td>
      <td>{{ item.nombre }}</td>
      <td>{{ item.tipo }}</td>
    </tr>
  </tbody>
</table>
</template>

<script>
export default {
    props:{
        datos: Array
    }
}
</script>