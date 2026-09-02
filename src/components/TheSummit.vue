<template>
  <section class="py-[32px] px-[16px] md:px-[32px] lg:p-0">
    <div
      class="bg-[#0B1C23]/70 p-[16px] md:p-[20px] lg:px-[42px] lg:py-[36px] rounded-[24px]"
    >
      <div>
        <ul
          ref="navScroll"
          class="flex items-center gap-3 overflow-x-auto lg:justify-between lg:gap-0 lg:overflow-visible scrollbar-hide"
          @wheel="handleWheel"
          @pointerdown="handlePointerDown"
          @pointermove="handlePointerMove"
          @pointerup="handlePointerUp"
          @pointercancel="handlePointerUp"
        >
          <li
            class="shrink-0 bg-[#0E1418] hover:bg-[#84FFC1] hover:text-[#121B26] border border-[#283437] py-[10px] px-[18px] rounded-full"
          >
            <a href="#incentives" class="font-[700] text-[18px] leading-[24px]">
              Enterprise Uzbekistan
            </a>
          </li>

          <li
            class="shrink-0 bg-[#0E1418] hover:bg-[#84FFC1] hover:text-[#121B26] border border-[#283437] py-[10px] px-[18px] rounded-full"
          >
            <a href="#incentives" class="font-[700] text-[18px] leading-[24px]">
              Startup & VC
            </a>
          </li>

          <li
            class="shrink-0 bg-[#0E1418] hover:bg-[#84FFC1] hover:text-[#121B26] border border-[#283437] py-[10px] px-[18px] rounded-full"
          >
            <a href="#incentives" class="font-[700] text-[18px] leading-[24px]">
              Service Companies
            </a>
          </li>

          <li
            class="shrink-0 bg-[#0E1418] hover:bg-[#84FFC1] hover:text-[#121B26] border border-[#283437] py-[10px] px-[18px] rounded-full"
          >
            <a href="#incentives" class="font-[700] text-[18px] leading-[24px]">
              Global Bridge
            </a>
          </li>

          <li
            class="shrink-0 bg-[#0E1418] hover:bg-[#84FFC1] hover:text-[#121B26] border border-[#283437] py-[10px] px-[18px] rounded-full"
          >
            <a href="#incentives" class="font-[700] text-[18px] leading-[24px]">
              Gamedev
            </a>
          </li>

          <li
            class="shrink-0 bg-[#0E1418] hover:bg-[#84FFC1] hover:text-[#121B26] border border-[#283437] py-[10px] px-[18px] rounded-full"
          >
            <a href="#incentives" class="font-[700] text-[18px] leading-[24px]">
              AI NATIVE
            </a>
          </li>
        </ul>
      </div>
      <h2
        class="font-[700] text-[26px] md:text-[36px] lg:text-[56px] leading-[120%] my-[20px] md:my-[24px] lg:my-[32px] md:text-center"
      >
        ENTERPRISE UZBEKISTAN SUMMIT
      </h2>
      <div
        class="grid grid-cols-3 bg-[#10171C]/70 rounded-[16px] px-[15px] py-[10px] border border-[#272E33]"
      >
        <div
          class="flex items-center gap-[10px] text-[12px] md:text-[14px] lg:text-[16px] font-[600] leading-[100%] border-r border-[#3D5960]"
        >
          <i class="bx bx-calendar text-[#84FFC1]" />
          <p>October 23, 2023</p>
        </div>
        <div
          class="flex items-center gap-[10px] text-[12px] md:text-[14px] lg:text-[16px] font-[600] leading-[100%] px-4 border-r border-[#3D5960]"
        >
          <i class="bx bx-clock-4 text-[#84FFC1]" />
          <p>10-00-12.00</p>
        </div>
        <div
          class="flex items-center gap-[10px] text-[12px] md:text-[14px] lg:text-[16px] font-[600] leading-[100%] px-4"
        >
          <i class="bx bx-location text-[#84FFC1]" />
          <p>CAEx, Hall 1</p>
        </div>
      </div>
      <div
        class="lg:flex gap-[32px] rounded-[16px] mt-[20px] md:mt-[24px] lg:mt-[32px]"
      >
        <div class="w-[100%]">
          <img
            src="../assets/images/summit.webp"
            alt="Summit"
            class="w-full rounded-[16px] lg:hidden"
            loading="lazy"
          />
          <div class="backimg filter-blur hidden lg:block grid"></div>
        </div>
        <div class="flex flex-col gap-[20px] my-[24px]">
          <h4
            class="text-[14px] md:text-[18px] font-[500] md:font-[600] leading-[150%]"
          >
            Discover Enterprise Uzbekistan — the country's first dedicated
            jurisdiction built for global technology business.
          </h4>
          <div class="flex items-center gap-[12px] text-[14px] lg:text-[16px]">
            <i
              class="bx bx-check bg-[#84FFC1] text-[#121B26] rounded-full"
            /><span
              >Running on elements of English and Welsh law, it offers a legal
              environment that locks in the day you enter and remains guaranteed
              through 2100 — for IT exporters, data centers, startups, and
              infrastructure and institutional investors alike.</span
            >
          </div>
          <div class="flex items-center gap-[12px] text-[14px] lg:text-[16px]">
            <i
              class="bx bx-check bg-[#84FFC1] text-[#121B26] rounded-full"
            /><span
              >On September 23, Enterprise Uzbekistan takes the stage at ICT
              Week to open the framework up in person. Meet the people building
              it, see how it's structured, and get a first look at what it means
              to operate inside it.</span
            >
          </div>
          <div class="flex items-center gap-[12px] text-[14px] lg:text-[16px]">
            <i
              class="bx bx-check bg-[#84FFC1] text-[#121B26] rounded-full"
            /><span
              >Join us at CAEx, Main Hall — come see it before everyone else
              does.</span
            >
          </div>
          <div
            class="flex items-center gap-[12px] bg-[#1F3737] border border-[#1D875F] rounded-[12px] px-[16px] py-[14px]"
          >
            <div class="w-[2px] bg-[#84FFC1] h-[20px]"></div>
            <p class="font-[600] text-[13px] lg:text-[18px]">
              Ideal for: global tech companies, investors, legal and financial
              advisors, and government officials
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref } from "vue";

const navScroll = ref(null);

let isDragging = false;
let startX = 0;
let startScrollLeft = 0;

const isMobileOrTablet = () => {
  return window.innerWidth < 1024;
};

const handleWheel = (event) => {
  if (!isMobileOrTablet()) return;

  const element = navScroll.value;

  if (!element) return;

  event.preventDefault();

  element.scrollLeft += event.deltaY || event.deltaX;
};

const handlePointerDown = (event) => {
  if (!isMobileOrTablet()) return;

  const element = navScroll.value;

  if (!element) return;

  isDragging = true;
  startX = event.clientX;
  startScrollLeft = element.scrollLeft;

  element.setPointerCapture(event.pointerId);
  element.style.cursor = "grabbing";
};

const handlePointerMove = (event) => {
  if (!isDragging || !isMobileOrTablet()) return;

  const element = navScroll.value;

  if (!element) return;

  const distance = event.clientX - startX;

  element.scrollLeft = startScrollLeft - distance;
};

const handlePointerUp = (event) => {
  if (!isDragging) return;

  const element = navScroll.value;

  if (!element) return;

  isDragging = false;

  if (element.hasPointerCapture(event.pointerId)) {
    element.releasePointerCapture(event.pointerId);
  }

  element.style.cursor = "";
};
</script>

<style lang="scss" scoped>
.scrollbar-hide {
  -ms-overflow-style: none;
  scrollbar-width: none;
  cursor: grab;
  touch-action: pan-x;
  user-select: none;
}

.scrollbar-hide::-webkit-scrollbar {
  display: none;
}

.backimg {
  background-image: url("../assets/images/summit.webp");
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  --webkit-backdrop-filter: blur(10px);
  height: 100%;
  width: 100%;
  padding: 20px;
}
</style>
