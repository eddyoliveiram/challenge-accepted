<template>
  <nav class="bg-blue-500 p-4 fixed top-0 left-0 right-0 z-10">
    <div class="container mx-auto flex justify-between items-center">
      <div class="text-white font-bold text-xl">
        <a href="#" class="hover:text-gray-300">MyWebsite</a>
      </div>
      <div class="flex space-x-4">
        <a href="/" class="text-white hover:text-gray-300">Home</a>
        <a href="/about" class="text-white hover:text-gray-300">About</a>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'NavbarStructure',
};
</script>

<style scoped>
/* Estilos adicionais, se necessário */
html, body {
  margin: 0;
  padding: 0;
  height: 100%;
}
</style>
