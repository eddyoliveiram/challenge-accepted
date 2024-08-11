<template>
  <RegisterForm/>

  <TableComponent/>

</template>

<script>
import RegisterForm from "@/components/RegisterForm.vue";
import TableComponent from "@/components/TableComponent.vue";

export default {
  name: 'HomePage',
  components: {TableComponent, RegisterForm}
}
</script>

