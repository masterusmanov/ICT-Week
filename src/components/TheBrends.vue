<template>
  <section
    class="py-[24px] md:py-0 px-[16px] md:px-[32px] md:py-[54px] lg:px-0"
  >
    <div
      class="border border-[#3D5960] bg-[#0B1C23] rounded-[16px] grid gap-[8px] md:gap-[12px] lg:gap-[32px] px-[16px] md:px-[32px] py-[32px] md:py-[54px]"
    >
      <h2
        class="text-[#EDEDF2] text-[24px] font-[700] md:text-[36px] lg:text-[48px] leading-[120%] text-center"
      >
        Past Attendees Include
      </h2>
      <div
        class="grid grid-cols-3 md:grid-cols-5 gap-[8px] md:gap-[12px] lg:gap-[32px] mt-[24px] lg:mt-[56px]"
      >
        <div
          v-for="brand in brands"
          :key="brand.id"
          class="border border-[#3D7A65] bg-[#0C1319] rounded-[10px] md:rounded-[10px] px-[32px] py-[18px] md:py-[24px] md:px-[33px] lg:py-[36px] lg:px-[26px] flex items-center justify-center"
        >
          <img
            :src="getImageUrl(brand.name)"
            :alt="brand.alt"
            width="160"
            height="64"
            class="w-full h-[36px] md:h-[48px] lg:h-[64px] object-contain"
            loading="lazy"
          />
        </div>
      </div>
      <div
        class="grid grid-cols-2 md:grid-cols-4 gap-[8px] md:gap-[12px] lg:gap-[32px]"
      >
        <div
          v-for="brand in brandTwoData"
          :key="brand.id"
          class="border border-[#3D7A65] bg-[#0C1319] rounded-[10px] md:rounded-[10px] px-[32px] py-[18px] md:py-[24px] md:px-[33px] lg:py-[36px] lg:px-[26px] flex items-center justify-center"
        >
          <img
            :src="getImageUrl(brand.name)"
            :alt="brand.alt"
            width="160"
            height="64"
            class="w-full h-[36px] md:h-[48px] lg:h-[64px] object-contain"
            loading="lazy"
          />
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref } from "vue";
import brandsData from "../data/branddata.json";
import brandTwo from "../data/brandtwo.json";

const brands = ref(brandsData);
const brandTwoData = ref(brandTwo);

const getImageUrl = (name) => {
  return new URL(`../assets/images/brands/${name}`, import.meta.url).href;
};
</script>

<style lang="scss" scoped></style>
