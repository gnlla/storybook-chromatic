<script setup lang="ts">
import { useCounterStore } from "@/stores/counter";

const count = useCounterStore();

const add = () => {
  count.increment();
};
</script>
<template>
  <div>
    {{ count.count }}

    <button @click="add">increment</button>
  </div>
</template>
