<template>
  <div id="app">
    <input type="text" @input="text = $event.target.value" :value="text" />
    {{ text }}

    <br />

    <input type="text2"  v-model="text2" />
    {{ text2 }}
  </div>
</template>

<script>
export default {
  name: "App",
  components: {},
  data() {
    return {
      text: "digite aqui -> campo input",
      text2: "digite aqui -> v-model",
    };
  },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
