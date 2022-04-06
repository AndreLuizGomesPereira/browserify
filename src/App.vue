<template>
  <div id="app">
    <my-menu title="My App">
      <ul>
        <li>Item 1</li>
        <li>Item 2</li>
        <li>Item 3</li>
      </ul>
    </my-menu>
    <h1>{{ msg }}</h1>
  </div>
</template>

<script>
import MyMenu from "./MyMenu.vue";
export default {
  components: { MyMenu },
  name: "app",
  data() {
    return {
      msg: "Olá Vue",
    };
  },
};
</script>

<style scoped>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

img {
  width: 200px;
  height: 200px;
}

h1,
h2 {
  font-weight: normal;
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
