<script setup>
import HeaderSection from './components/HeaderSection.vue'
import ContactSection from './components/ContactSection.vue'
import MediaSection from './components/MediaSection.vue'
import LanguageSection from './components/LanguageSection.vue'
import SkillBar from './components/SkillBar.vue'
import ExperienceItem from './components/ExperienceItem.vue'
// import html2pdf from 'html2pdf.js'

// const pdfGen = () => {
//   const myCvSpa = document.getElementsByClassName('myCv');
// html2pdf().from(myCvSpa).save('My_Vue_App_CV.pdf');
// }

</script>

<template>
  <div class="myCv">
    <div class="bg-gray-200 w-full flex flex-col items-center p-2 min-h-screen justify-center">
      <div
        class="bg-white min-h-screen p-10 w-full md:w-full lg:w-[60%] gap-20 flex flex-col items-center relative"
      >
        <!-- Contours colorés de la page -->
        <div
          class="hidden lg:block absolute -top-45 left-45 rotate-90 h-[30%] border-l-31 border-[#00959C]"
        ></div>
        <div
          class="hidden lg:block absolute -top-0 right-0 h-[51%] border-l-40 border-[#00959C]"
        ></div>
        <div
          class="hidden lg:block absolute -bottom-62 left-61 h-[40%] border-l-30 border-[#00959C] rotate-90"
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
                <div class="p-4 hover:shadow-md leading-tight">
                  <!-- SOCIAL MEDIA -->
                  <h2
                    class="text-lg md:text-xl font-black text-gray-700 leading-[1] tracking-wide font-poppins name pb-3 pl-4 md:pl-7"
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
                        <p class="font-semibold text-gray-700 font-poppins">DRAWING</p>
                        <SkillBar pourcentage="55" />
                      </div>
                    </div><br>
                  </div>

                  <!-- PHOTO -->
                  <div class="mb-6 relative pl-7 border-l-2 border-[#00959C]">
                    <div class="absolute -left-1 top-2 w-2 h-2 rounded-full bg-[#00959C]"></div>
                    <div class="flex gap-4 items-center">
                      <div class="w-full">
                        <p class="font-semibold text-gray-700 font-poppins">PHOTO</p>
                        <SkillBar pourcentage="70" />
                      </div>
                    </div><br>
                  </div>

                  <!-- COPYWRITE -->
                  <div class="mb-6 relative pl-7 border-l-2 border-[#00959C]">
                    <div class="absolute -left-1 top-2 w-2 h-2 rounded-full bg-[#00959C]"></div>
                    <div class="flex gap-4 items-center">
                      <div class="w-full">
                        <p class="font-semibold text-gray-700 font-poppins">COPYWRITE</p>
                        <SkillBar pourcentage="80" />
                      </div>
                    </div><br>
                  </div>
                  <!-- COMPUTERIZE -->
                  <div class="mb-6 relative pl-7 border-l-2 border-[#00959C]">
                    <div class="absolute -left-1 top-2 w-2 h-2 rounded-full bg-[#00959C]"></div>
                    <div class="flex gap-4 items-center">
                      <div class="w-full">
                        <p class="font-semibold text-gray-700 font-poppins">COMPUTERIZE</p>
                        <SkillBar pourcentage="80" />
                      </div>
                    </div><br>
                  </div>

                  <!-- DESIGN -->
                  <div class="mb-6 relative pl-7 border-l-2 border-[#00959C]">
                    <div class="absolute -left-1 top-2 w-2 h-2 rounded-full bg-[#00959C]"></div>
                    <div class="flex gap-4 items-center">
                      <div class="w-full">
                        <p class="font-semibold text-gray-700 font-poppins">DESIGN</p>
                        <SkillBar pourcentage="50" />
                      </div>
                    </div><br>
                  </div>
                </div>
              </div>
            </div>

            <div class="md:col-span-2 bg-white pl-5 hover:shadow-md md:row-span-2">
              <div class="md:col-span-1">
                <div class="p-4">
                  <h2
                    class="text-xl font-black text-gray-700 leading-[0.5] tracking-wide font-poppins pl-9 name"
                  >
                    EXPERIENCE
                  </h2>
                  <div class="mb-6 relative pl-7 border-l-2 border-[#00959C] py-2">
                    <div class="absolute -left-1 -top-1 w-2 h-2 rounded-full bg-[#00959C]"></div>
                  </div>
                  <div class="mb-6 relative pl-7 border-l-2 border-[#00959C]">
                    <div class="absolute -left-1 top-2 w-2 h-2 rounded-full bg-[#00959C]"></div>
                    <div class="flex gap-4 items-center">
                      <div class="w-full">
                        <ExperienceItem
                          -main-title="JOB POSITION"
                          -sub-title="COMPANY NAME 2020 | 2021"
                          -description="Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam,"
                        />
                      </div>
                    </div>
                  </div>
                  <div class="mb-6 relative pl-7 border-l-2 border-[#00959C]">
                    <div class="absolute -left-1 top-2 w-2 h-2 rounded-full bg-[#00959C]"></div>
                    <div class="flex gap-4 items-center">
                      <div class="w-full">
                        <ExperienceItem
                          -main-title="JOB POSITION"
                          -sub-title="COMPANY NAME 2020 | 2021"
                          -description="Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam,"
                        />
                      </div>
                    </div>
                  </div>
                  <div class="mb-6 relative pl-7 border-l-2 border-[#00959C]">
                    <div class="absolute -left-1 top-2 w-2 h-2 rounded-full bg-[#00959C]"></div>
                    <div class="flex gap-4 items-center">
                      <div class="w-full">
                        <ExperienceItem
                          -main-title="JOB POSITION"
                          -sub-title="COMPANY NAME 2020 | 2021"
                          -description="Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam,"
                        />
                      </div>
                    </div>
                  </div>
                  <div class="pt-5">
                    <hr class="border-0 bg-[#00959C] w-[90%] h-[2px] mt-4" />
                  </div>
                </div>
              </div>

              <div class="cols-span-2">
                <div class="p-4">
                  <h2
                    class="text-xl font-black text-gray-700 leading-[0.5] tracking-wide font-poppins pl-9 name"
                  >
                    EXPERIENCE
                  </h2>
                  <div class="mb-6 relative pl-7 border-l-2 border-[#00959C] py-2">
                    <div class="absolute -left-1 -top-1 w-2 h-2 rounded-full bg-[#00959C]"></div>
                  </div>
                  <div class="mb-6 relative pl-7 border-l-2 border-[#00959C]">
                    <div class="absolute -left-1 top-2 w-2 h-2 rounded-full bg-[#00959C]"></div>
                    <div class="flex gap-4 items-center">
                      <div class="w-full">
                        <ExperienceItem
                          -main-title="MASTER DEGREE"
                          -sub-title="UNIVERSITY NAME 2020 | 2021"
                          -description="Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam,"
                        />
                      </div>
                    </div>
                  </div>
                  <div class="mb-6 relative pl-7 border-l-2 border-[#00959C]">
                    <div class="absolute -left-1 top-2 w-2 h-2 rounded-full bg-[#00959C]"></div>
                    <div class="flex gap-4 items-center">
                      <div class="w-full">
                        <ExperienceItem
                          -main-title="MASTER DEGREE"
                          -sub-title="UNIVERSITY NAME 2020 | 2021"
                          -description="Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam,"
                        />
                      </div>
                    </div>
                  </div>
                  <div class="mb-6 relative pl-7 border-l-2 border-[#00959C]">
                    <div class="absolute -left-1 top-2 w-2 h-2 rounded-full bg-[#00959C]"></div>
                    <div class="flex gap-4 items-center">
                      <div class="w-full">
                        <ExperienceItem
                          -main-title="MASTER DEGREE"
                          -sub-title="UNIVERSITY NAME 2020 | 2021"
                          -description="Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam,"
                        />
                      </div>
                    </div>
                  </div>
                </div>
              </div>
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
