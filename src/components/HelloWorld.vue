<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>
      Sigue la siguiente
      <a href="https://lamapacha.net/" target="_blank" rel="noopener">guia</a>
      para comenzar a mapachear.
    </p>
    <input type="text" v-model="nombre" placeholder="Escribe tu nombre">
    <p>Hola <strong>{{nombre}}</strong></p>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String,
  },
  data() {
    return {
      nombre: '',
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
