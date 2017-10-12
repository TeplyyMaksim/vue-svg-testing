<template>
  <div id="app">
    <img src="./assets/logo.png">
    <icon-component/>
  </div>
</template>

<script>
import IconComponent from './components/IconComponent';

export default {
  name: 'app',
  components: {
    IconComponent,
  },
};
</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  /* Global font-sizing */
  font-size: 16px;
}
</style>
