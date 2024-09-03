<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <PrimerComponent titulo="Hola mundo en vue" 
  nombre="Ahmad"
  v-bind:edad="24" 
  v-bind:src="require('@/assets/AhmadAstro.jpg')"
  v-bind:imagenStyle="{ width: '100px', height: 'auto' }" />
</template>

<script>
import PrimerComponent from './components/primerComponent.vue';

export default {
  name: 'App',
  components: {
    PrimerComponent,
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
