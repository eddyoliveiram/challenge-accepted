<template>
  <RegisterForm/>
  <TableComponent/>
</template>

<script>
import RegisterForm from "@/components/base/LoginForm.vue";
import TableComponent from "@/components/base/TableComponent.vue";

export default {
  name: 'HomePage',
  components: {TableComponent, RegisterForm}
}
</script>

