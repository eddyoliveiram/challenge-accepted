<template>
  <div id="app">
    <NavbarStructure />
    <router-view />
  </div>
</template>

<script>
import NavbarStructure from "@/components/layout/NavbarStructure.vue";

export default {
  name: 'App',
  components: {
    NavbarStructure,
  },
};
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Open+Sans:300,400,600,700');

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
