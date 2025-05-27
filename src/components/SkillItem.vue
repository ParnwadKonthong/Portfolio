<template>
  <div
    class="w-auto p-2 border border-gray-300 rounded-3xl shadow-md bg-white/72 text-center flex items-center gap-2"
  >
    <img :src="icon" class="w-8 h-8" />
    <div class="font-bold text-base">{{ name }}</div>
  </div>
</template>

<script setup>
defineProps({
  icon: String,
  name: String,
});
</script>
