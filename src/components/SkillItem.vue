<template>
  <div
    class="w-auto p-2 px-6 border border-gray-300 rounded-3xl shadow-md bg-white/72 text-center flex items-center gap-2"
  >
    <img v-if="icon" :src="icon" class="w-8 h-8" />
    <div :class="icon ? 'font-bold text-base' : 'font-bold text-base mx-auto'">{{ name }}</div>
  </div>
</template>

<script setup lang="ts">
defineProps<{
  icon?: string;
  name: string;
}>();
</script>
