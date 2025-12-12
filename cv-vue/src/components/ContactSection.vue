<template>
  <div class="flex flex-col md:flex-row gap-5 md:gap-5 items-center">
    <div class="w-full md:w-1/3">
      <h2
        class="text-xl font-black text-gray-700 leading-[1] tracking-wide font-poppins name pb-3 pl-7"
      >
        CONTACT
      </h2>
      <div
        class="border-2 border-b-transparent border-r-transparent border-t-transparent border-l-[#00959C] pl-5 gap-1"
      >
        <div></div>
        <!-- Phone -->
        <div class="flex items-center gap-5">
          <div class="text-[#00959C] text-2xl">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 24 24"
              fill="currentColor"
              class="size-6"
            >
              <path d="M10.5 18.75a.75.75 0 0 0 0 1.5h3a.75.75 0 0 0 0-1.5h-3Z" />
              <path
                fill-rule="evenodd"
                d="M8.625.75A3.375 3.375 0 0 0 5.25 4.125v15.75a3.375 3.375 0 0 0 3.375 3.375h6.75a3.375 3.375 0 0 0 3.375-3.375V4.125A3.375 3.375 0 0 0 15.375.75h-6.75ZM7.5 4.125C7.5 3.504 8.004 3 8.625 3H9.75v.375c0 .621.504 1.125 1.125 1.125h2.25c.621 0 1.125-.504 1.125-1.125V3h1.125c.621 0 1.125.504 1.125 1.125v15.75c0 .621-.504 1.125-1.125 1.125h-6.75A1.125 1.125 0 0 1 7.5 19.875V4.125Z"
                clip-rule="evenodd"
              />
            </svg>
          </div>

          <div class="gap-1 text-nowrap leading-none">
            <p class="font-semibold text-gray-700 font-poppins">Phone</p>
            <p class="text-gray-700 font-poppins">{{ phoneNumber }}</p>
          </div>
        </div>
        <div class="h-2"> </div>
        <!-- Email -->
        <div class="flex items-center gap-5">
          <div class="text-[#00959C] text-2xl">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 24 24"
              fill="currentColor"
              class="size-6"
            >
              <path
                d="M1.5 8.67v8.58a3 3 0 0 0 3 3h15a3 3 0 0 0 3-3V8.67l-8.928 5.493a3 3 0 0 1-3.144 0L1.5 8.67Z"
              />
              <path
                d="M22.5 6.908V6.75a3 3 0 0 0-3-3h-15a3 3 0 0 0-3 3v.158l9.714 5.978a1.5 1.5 0 0 0 1.572 0L22.5 6.908Z"
              />
            </svg>
          </div>
          <div class="flex flex-col leading-none">
            <p class="font-semibold text-gray-700 font-poppins">Email</p>
            <p class="text-gray-700 text-nowrap font-poppins">{{ emailAdress }}</p>
          </div>
        </div>
      </div>
    </div>

    <!-- BARRE VERTICALE — même couleur que dans l’image -->
    <div class="hidden md:block w-[3px] bg-[#00959C] h-full"></div>

    <!-- ABOUT ME (colonne droite) -->
    <div class="w-full md:w-2/3">
      <h2
        class="text-xl font-black text-gray-700 leading-[0.5] tracking-wide font-poppins name pb-4 pl-5"
      >
        ABOUT ME
      </h2>

      <div class="mt-4 flex gap-4 p-2">
        <hr class="hidden md:block border-[#00959C] border-[1.5px] h-auto rotate-0" />
        <p class="text-gray-700 leading-none text-justify font-poppins">{{ aboutDesc }}</p>
      </div>
    </div>
  </div>
</template>

<script setup>
defineProps({
  phoneNumber: String,
  emailAdress: String,
  aboutDesc: String,
})
</script>
<style scoped>
.name {
  font-weight: 600;
}
</style>
