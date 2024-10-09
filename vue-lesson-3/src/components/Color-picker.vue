<script setup>

const model = defineModel();

</script>

<template>
  <input type="color" v-model="model" />
</template>

<style scoped>
input {
  width: 30%;
  height: 50%;
}
</style>
