<script setup>
import { ref, setBlockTracking } from "vue";
import Card from "./components/Card.vue";
import ColorPicker from "./components/Color-picker.vue";


const currentColor = ref("#323232");

defineProps({
  type: String,
});
</script>

<template>
  <div class="board">
    <Card :color="currentColor"> </Card>
    <ColorPicker v-model="currentColor"></ColorPicker>
  </div>
</template>

<style scoped>
.board {
  width: 80vw;
  height: 60vh;
  background-color: #083344;

  padding: 20px;
  display: flex;
  justify-content: space-between;
}
</style>
