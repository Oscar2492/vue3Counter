<template>
  <Grid>
    <img :src="url" :alt="nombre" />
    <h2>vue.js</h2>
    <a :href="url" target="_blank">Download</a>
    <a :href="url" target="_blank">Visitar</a>
  </Grid>
</template>
<script>
import Grid from "./Grid.vue";

export default {
  props: {
    url: {
      String,
    },
    nombre: {
      String,
    },
  },
  components: { Grid },
};
</script>

<style scoped>
img {
  width: 8rem;
  height: 8rem;
}
a {
  color: white;
  text-decoration: none;
  columns: snow;
  background: #301675;
  padding: 0.3rem;
  border-radius: 5px;
  border: 1px solid #f2f2f2;
}
</style>
