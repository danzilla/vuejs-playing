<template>
  <div id="app">
    <b-container>
      <img src="./assets/logo.png" />
      <h1>{{ msg }}</h1>

      <b-button-group>
        <b-button variant="success">Success</b-button>
        <b-button variant="primary">Info</b-button>
        <b-button variant="warning">Warning</b-button>
      </b-button-group>

      <HelloWorld msg="Welcome to Your Vue.js App" />

    </b-container>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: "app",
  components: {
    HelloWorld
  },
  data() {
    return {
      msg: "Vue.js -> vue 2.x and bootstrap 4",
    };
  },
};
</script>

<style lang="scss">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
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
