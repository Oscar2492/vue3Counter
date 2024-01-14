<template>
  <form @submit.prevent="addUser()">
    <div>
      <label
        >Nombre:
        <input v-model="nombre" type="text" placeholder="Nombre" required />
      </label>
    </div>
    <div>
      <label
        >Edad:
        <input
          v-model="edad"
          type="number"
          min="15"
          max="100"
          placeholder="Edad"
          required
        />
      </label>
    </div>
    <div>
      <label
        >Email:
        <input v-model="mail" type="email" placeholder="email" required />
      </label>
    </div>

    <button type="submit">Submit</button>
  </form>
</template>
<script>
export default {
  data() {
    return {
      nombre: "",
      edad: 0,
      mail: "",
    };
  },
  methods: {
    addUser() {
      console.log(this.nombre, this.edad, this.mail);
    },
  },
};
</script>
