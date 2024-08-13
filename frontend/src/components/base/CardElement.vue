<template>
  <div class="card w-full max-w-sm shadow-lg">
    <div class="card-body">
      <h2 class="card-title text-lg">{{ title }}</h2>
      <slot></slot>
    </div>
  </div>
</template>

<script>
export default {
  name: 'CardElement',
  props: {
    title: {
      type: String,
      required: true
    }
  }
};
</script>

<style scoped>
</style>
