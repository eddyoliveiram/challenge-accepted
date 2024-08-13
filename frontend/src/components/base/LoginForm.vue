<template>
  <div class="min-h-screen flex items-center justify-center">
      <CardElement title="Login">
        <form @submit.prevent="submitForm">
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
            <PrimaryButton :value="'Login'" />
            <SecondaryButton
                :value="'Clear'"
                @click="clearForm"
                extraClasses="mt-1"
            />
          </div>
        </form>
      </CardElement>
  </div>
</template>

<script>
import FormInput from '@/components/base/FormInput.vue';
import CardElement from "@/components/base/CardElement.vue";
import SecondaryButton from "@/components/base/SecondaryButton.vue";
import PrimaryButton from "@/components/base/PrimaryButton.vue";

export default {
  name: 'RegisterForm',
  components: {
    PrimaryButton,
    SecondaryButton,
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
