<template>
  <button
      type="submit"
      :class="['btn', 'btn-primary', extraClasses]"
      :value="value"
  >
    {{ value }}
  </button>
</template>

<script>
export default {
  name: 'PrimaryButton',
  props: {
    value: {
      type: String,
      required: true
    },
    extraClasses: {
      type: String,
      default: ''
    }
  }
};
</script>
