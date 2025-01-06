<template>
  <button
    class="px-3 py-2 rounded-full w-40 border-2 text-white border-emerald-600 bg-emerald-500 hover:bg-emerald-600 transition-colors"
  >
    <slot></slot>
  </button>
</template>

<script setup>
const props = defineProps({
  title: String,
});
</script>
