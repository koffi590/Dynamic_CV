<template>
  <div>
    <div class="leading-none">
      <h1 class="font-semibold text-gray-900 font-poppins main">{{ MainTitle }}</h1>
      <h1 class="sub text-[#00959C] font-poppins pb-3">{{ SubTitle }}</h1>
    </div>
    <p class="text-normal text-gray-700 font-poppins pb-3">{{ Description }}</p>
  </div>
</template>
<script setup>
defineProps({
  MainTitle: String,
  SubTitle: String,
  Description: String,
})
</script>
<style scoped>
.sub {
  font-size: 10;
}
</style>
