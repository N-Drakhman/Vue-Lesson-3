<script setup>


const props = defineProps({
  color: String,
});


</script>

<template>
  <div class="card" :style="{ backgroundColor: color || 'blue' }">
  </div>
  <span>{{ color || "no color" }}</span>
</template>

<style scoped>
.card {
  width: 30%;
  height: 50%;
  padding: 25px;
  background-color: blue;
}

span {
  color: darkgrey;
  font-weight: bold;
  font-size: 18px;
}
</style>
