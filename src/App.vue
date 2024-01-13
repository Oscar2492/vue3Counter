<script>
export default {
  data: () => ({
    contador: 10,
  }),
  methods: {
    incrementar() {
      this.contador += 1;
    },
    disminuir() {
      this.contador -= 1;
    },
    reset() {
      this.contador = 10;
    },
  },
};
</script>
<template>
  <div class="container">
    <img src="./assets/logo.svg" alt="logo" width="100" height="100" />
    <h1>hola mundo</h1>
    <hr />
    <h2>Contador: {{ contador }}</h2>
    <button @click="incrementar">+1</button>
    <button @click="disminuir">-1</button>
    <button @click="reset">Reset</button>
  </div>
</template>

<style scoped>
.container {
  text-align: center;
}
</style>
