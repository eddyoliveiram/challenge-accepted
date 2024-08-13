<template>
  <button
      type="button"
      :class="['btn', 'neutral-content', extraClasses]"
      :value="value"
      @click="onClick"
  >
    {{ value }}
  </button>
</template>

<script>
export default {
  name: 'SecondaryButton',
  props: {
    value: {
      type: String,
      required: true
    },
    extraClasses: {
      type: String,
      default: ''
    }
  },
  methods: {
    onClick() {
      this.$emit('click');
    }
  }
};
</script>
