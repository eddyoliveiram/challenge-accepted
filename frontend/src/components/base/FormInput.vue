<template>
  <div class="form-control">
    <label class="label">
      <span class="label-text text-sm">{{ label }}</span>
    </label>
    <input
        :type="type"
        :placeholder="placeholder"
        class="input input-bordered text-base"
        v-model="inputValue"
    />
  </div>
</template>

<script>
export default {
  name: 'FormInput',
  props: {
    label: {
      type: String,
      required: true
    },
    type: {
      type: String,
      required: true,
      default: 'text'
    },
    placeholder: {
      type: String,
      required: true
    },
    modelValue: {
      type: String,
      required: true
    }
  },
  computed: {
    inputValue: {
      get() {
        return this.modelValue;
      },
      set(value) {
        this.$emit('update:modelValue', value);
      }
    }
  }
};
</script>

<style scoped>
</style>
