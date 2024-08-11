<template>
  <div class="min-h-screen bg-gray-100 flex items-center justify-center">
      <CardElement title="Register">
        <form @submit.prevent="submitForm">
          <FormInput
              label="Name"
              type="text"
              placeholder="Enter your name"
              v-model="formData.name"
          />
          <FormInput
              label="Email"
              type="email"
              placeholder="Enter your email"
              v-model="formData.email"
          />
          <FormInput
              label="Password"
              type="password"
              placeholder="Enter your password"
              v-model="formData.password"
          />
          <div class="form-control mt-6">
            <button type="submit" class="btn btn-primary text-base">Register</button>
          </div>
        </form>
      </CardElement>
  </div>
</template>

<script>
import FormInput from '@/components/base/FormInput.vue';
import CardElement from "@/components/base/CardElement.vue";

export default {
  name: 'RegisterForm',
  components: {
    CardElement,
    FormInput
  },
  data() {
    return {
      formData: {
        name: '',
        email: '',
        password: ''
      }
    };
  },
  methods: {
    submitForm() {
      console.log('Form submitted:', this.formData);
    }
  }
};
</script>

<style scoped>
</style>
