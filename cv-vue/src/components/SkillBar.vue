<script setup>
defineProps({
  pourcentage: {
    type: Number,
    required: true
  }
})
</script>
<template>
  <div class="w-full bg-gray-200 h-2 overflow-hidden">
    <div
      class="h-full bg-[#00959C] transition-all duration-500"
      :style="{ width: pourcentage + '%' }"
    ></div>
  </div>
</template>

