<script setup>
const items = [
  {
    title: "first",
    description: "Lorem 1",
  },
  {
    title: "second",
    description: "Lorem 2",
  },
  {
    title: "third",
    description: "Lorem 3",
  },
];

const emit = defineEmits(['accordion:click'])
</script>

<template>
    <div class="accordion">
        <div class="accordion-item" v-for="item in items" :key="item.title" @click="emit('accordion:click')">
            <h3>{{ item.title }}</h3>
            <p>{{ item.description }}</p>
        </div>
    </div>
</template>


<style>
p{
    color: red
}
</style>