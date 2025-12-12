<script setup>
import HeaderSection from './components/HeaderSection.vue'
import ContactSection from './components/ContactSection.vue'
import MediaSection from './components/MediaSection.vue'
import LanguageSection from './components/LanguageSection.vue'
import SkillBar from './components/SkillBar.vue'
import ExperienceItem from './components/ExperienceItem.vue'
</script>

<template>
  <div class="">
    <div class="bg-gray-200 w-full flex flex-col items-center p-2 min-h-screen justify-center">
      <div
        class="bg-white min-h-screen p-10 w-full md:w-full lg:w-[60%] gap-20 flex flex-col items-center relative"
      >
        <!-- Contours colorés de la page -->
        <div
          class="hidden lg:block absolute -top-43 left-43 rotate-90 h-[30%] border-l-23 border-[#00959C]"
        ></div>
        <div
          class="hidden lg:block absolute -top-0 right-0 h-[51%] border-l-24 border-[#00959C]"
        ></div>
        <div
          class="hidden lg:block absolute -bottom-59 left-58 h-[40%] border-l-24 border-[#00959C] rotate-90"
        ></div>

        <!-- PHOTO DE PROFIL + NOM -->
        <div class="">
          <HeaderSection user-name="NAME" user-surname="SURNAME" user-profession="PROFESSION" />
          <div class="w-full p-6">
            <!-- CONTACTS + ABOUT -->
            <div class="pb-4">
              <ContactSection
                phone-number="+2 434–232–534234"
                email-adress="travis.anderson@mail.com"
                about-desc="
          Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod
          tincidunt ut laoreet dolore magna aliquam erat volutpat. Ut wisi enim ad"
              />
            </div>
            <div class="flex items-center justify-center">
              <hr class="border-0 bg-[#00959C] w-[98%] h-[2px] mt-4" />
            </div>
          </div>
          <div class="grid grid-cols-1 md:grid-cols-3 grid-flow-row-dense gap-4 p-2">
            <div>
              <!-- RESEAUX SOCIAUX -->
              <div class="md:col-span-1 hover:shadow-md">
                <MediaSection />
              </div>

              <!-- LANGUES -->
              <div class="md:col-span-1 hover:shadow-md">
                <LanguageSection />
              </div>

              <div class="md:col-span-1">
                <div class="p-4 hover:shadow-md">
                  <!-- SOCIAL MEDIA -->
                  <h2
                    class="text-xl font-black text-gray-700 leading-tight tracking-wide font-poppins pl-9 name"
                  >
                    PRO SKILLS
                  </h2>
                  <div class="mb-6 relative pl-7 border-l-2 border-[#00959C] py-2">
                    <div class="absolute -left-1 -top-1 w-2 h-2 rounded-full bg-[#00959C]"></div>
                  </div>
                  <!-- DRAWING -->
                  <div class="mb-6 relative pl-7 border-l-2 border-[#00959C]">
                    <div class="absolute -left-1 top-2 w-2 h-2 rounded-full bg-[#00959C]"></div>
                    <div class="flex gap-4 items-center">
                      <div class="w-full">
                        <p class="font-semibold text-gray-700">DRAWING</p>
                        <SkillBar pourcentage="55" />
                      </div>
                    </div>
                  </div>

                  <!-- PHOTO -->
                  <div class="mb-6 relative pl-7 border-l-2 border-[#00959C]">
                    <div class="absolute -left-1 top-2 w-2 h-2 rounded-full bg-[#00959C]"></div>
                    <div class="flex gap-4 items-center">
                      <div class="w-full">
                        <p class="font-semibold text-gray-700">PHOTO</p>
                        <SkillBar pourcentage="70" />
                      </div>
                    </div>
                  </div>

                  <!-- COPYWRITE -->
                  <div class="mb-6 relative pl-7 border-l-2 border-[#00959C]">
                    <div class="absolute -left-1 top-2 w-2 h-2 rounded-full bg-[#00959C]"></div>
                    <div class="flex gap-4 items-center">
                      <div class="w-full">
                        <p class="font-semibold text-gray-700">COPYWRITE</p>
                        <SkillBar pourcentage="80" />
                      </div>
                    </div>
                  </div>
                  <!-- COMPUTERIZE -->
                  <div class="mb-6 relative pl-7 border-l-2 border-[#00959C]">
                    <div class="absolute -left-1 top-2 w-2 h-2 rounded-full bg-[#00959C]"></div>
                    <div class="flex gap-4 items-center">
                      <div class="w-full">
                        <p class="font-semibold text-gray-700">COMPUTERIZE</p>
                        <SkillBar pourcentage="80" />
                      </div>
                    </div>
                  </div>

                  <!-- DESIGN -->
                  <div class="mb-6 relative pl-7 border-l-2 border-[#00959C]">
                    <div class="absolute -left-1 top-2 w-2 h-2 rounded-full bg-[#00959C]"></div>
                    <div class="flex gap-4 items-center">
                      <div class="w-full">
                        <p class="font-semibold text-gray-700">DESIGN</p>
                        <SkillBar pourcentage="50" />
                      </div>
                    </div>
                  </div>
                  <div class="pt-4">
                    <hr class="border-0 bg-[#00959C] w-[98%] h-[2px] mt-4" />
                  </div>
                </div>
              </div>
            </div>

            <!-- Colonne droite (prendre 2 colonnes, hauteur auto sur plusieurs lignes) -->
            <div class="md:col-span-2 bg-white pl-5 hover:shadow-md md:row-span-2">
              <div class="md:col-span-1">
                <div class="p-4">
                  <h2
                    class="text-xl font-black text-gray-700 leading-tight tracking-wide font-poppins pl-9 name"
                  >
                    EXPERIENCE
                  </h2>
                  <div class="mb-6 relative pl-7 border-l-2 border-[#00959C]">
                    <div class="absolute -left-1 top-2 w-2 h-2 rounded-full bg-[#00959C]"></div>
                    <div class="flex gap-4 items-center">
                      <div class="w-full">
                        <ExperienceItem />
                      </div>
                    </div>
                  </div>
                </div>
              </div>
              <div class="cols-span-2"></div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<style scoped>
.name {
  font-weight: 600;
}
</style>
