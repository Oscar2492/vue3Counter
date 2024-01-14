<template>
  <div class="counter">
    <Counter />
  </div>
  <div class="componentes">
    <h1>Componentes</h1>
    <Card
      url="https://cdn.svgporn.com/logos/vue.svg?response-content-disposition=attachment%3Bfilename%3Dvue.svg"
      nombre="Vue.js"
    />
    <Card
      url="https://cdn.svgporn.com/logos/vuetifyjs.svg?response-content-disposition=attachment%3Bfilename%3Dvuetifyjs.svg"
      nombre="Vuetify"
    />
    <Card
      url="https://cdn.svgporn.com/logos/angular-icon.svg?response-content-disposition=attachment%3Bfilename%3Dangular-icon.svg"
      nombre="Angular"
    />
    <Card
      url="https://cdn.svgporn.com/logos/react.svg?response-content-disposition=attachment%3Bfilename%3Dreact.svg"
      nombre="React"
    />
  </div>
  <div class="directivas">
    <h1>Directivas</h1>
    <Form />
  </div>
</template>

<script>
import Card from "./components/ComponentBasics/Card.vue";
import Counter from "./components/counter/Counter.vue";
import Form from "./components/formularios/Form.vue";
export default {
  components: {
    Card,
    Form,
    Counter,
  },
};
</script>
<style scoped>
.componentes {
  border-bottom: 3px solid black;
  padding-bottom: 25px;
}
.directivas {
  border-bottom: 3px solid black;
  padding-bottom: 25px;
}
</style>
