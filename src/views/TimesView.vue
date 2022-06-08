<script>
export default {
  data() {
    return {
      times: [
        { id: 1, name: "time1" },
        { id: 2, name: "time2" },
        { id: 3, name: "time3" },
        { id: 4, name: "time4" },
      ],
    };
  },
};
</script>
<template>
  <div class="container">
    <div class="title">
      <h2>Gerenciamento de times</h2>
    </div>
    <div class="form-input">
      <input type="text" />
      <button class="btnsalvar">Salvar</button>
    </div>
  </div>
  <div class="list-times">
    {{ times }}
    <table>
      <thead>
        <tr>
          <td>ID</td>
          <td>Nome</td>
          <td>Ações</td>
          <td>Time</td>
        </tr>
      </thead>

      <tbody>
        <tr v-for="time in times" :key="time.id">
          <td>{{ time.id }}</td>
          <td>{{ time.name }}</td>
          <td>???</td>
          <td></td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<style></style>
