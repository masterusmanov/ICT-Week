<template>
  <section
    class="py-[32px] px-[16px]  md:px-[32px] md:py-[54px] lg:px-0"
  >
    <div>
      <h1
        class="w-full lg:w-[944px] mx-auto text-[32px] md:text-[42px] lg:text-[70px] font-[800] md:font-[700] leading-[115%] md:leading-[120%] text-center my-[12px] md:my-[24px] lg:my-[28px]"
      >
        Unlock the World's Fastest Growing Ecosystem
      </h1>
      <p
        class="md:hidden text-[14px] leading-[150%] text-center text-[#B2B7B8] my-[12px]"
      >
        Learn everything about the thriving Uzbek tech ecosystem — in just one
        week. Meet 10k+ attendees, global VCs & partners.
      </p>
    </div>

    <div
      class="w-full grid lg:grid-cols-[3.5fr_2fr] gap-4 my-[24px] lg:my-[56px]"
    >
      <div
        class="w-full aspect-video rounded-2xl overflow-hidden mx-auto p-[2px]"
        style="
          background:
            radial-gradient(
              ellipse at top center,
              rgba(255, 255, 255, 0.8) 0%,
              transparent 70%
            ),
            linear-gradient(to right, #24433d 0%, #152522 50%, #24433d 100%);
        "
      >
        <iframe
          class="w-full h-full border-0 rounded-2xl"
          src="https://www.youtube.com/embed/NPhwTOz7AVw?si=KwnaVPHu90PJz47q"
          title="YouTube video player"
          allow="
            accelerometer;
            autoplay;
            clipboard-write;
            encrypted-media;
            gyroscope;
            picture-in-picture;
            web-share;
          "
          referrerpolicy="strict-origin-when-cross-origin"
          allowfullscreen
        ></iframe>
      </div>
      <div
        class="w-full bg-[#0B1C23]/45 my-[24px] lg:my-0 p-[16px] lg:p-[24px] border border-[#3D5960] rounded-[24px]"
      >
        <div
          class="w-full flex flex-col md:flex-row lg:flex-col items-center justify-between gap-10 rounded-[24px]"
        >
          <div class="flex-1 flex flex-col gap-4 order-2 md:order-1 lg:order-2">
            <p
              class="text-[16px] md:text-[20px] lg:text-[22px] leading-[120%] font-[500]"
            >
              Learn everything about the thriving Uzbek tech ecosystem — in just
              one week
            </p>
            <div
              class="flex items-center justify-center md:justify-start gap-2 md:gap-4 flex-wrap"
            >
              <button
                class="p-[12px] flex items-center gap-1 border border-[#62ECC4] text-[#62ECC4] hover:bg-[#62ECC4] hover:text-black font-semibold rounded-[12px] text-[16px] lg:text-[18px]"
              >
                Register now ↗
              </button>
              <button
                class="p-[12px] flex items-center gap-2 border border-[#62ECC4] text-[#62ECC4] hover:bg-[#62ECC4] hover:text-black font-semibold rounded-[12px] text-[16px] lg:text-[18px]"
              >
                <i class="bx bx-arrow-in-down-square-half text-[24px]" aria-hidden="true" />
                Full agenda
              </button>
            </div>
          </div>
          <div
            class="w-full max-w-[326px] md:max-w-[300px] lg:max-w-[560px] flex-shrink-0 order-1 md:order-2 lg:order-1"
          >
            <picture class="w-full block">
              <source
                media="(min-width: 1024px)"
                srcset="../assets/images/firstpic.webp"
              />
              <img
                src="../assets/images/secondpic.webp"
                alt="Event Preview"
                class="w-full h-[233px] md:h-[136px] object-cover rounded-[24px]"
              />
            </picture>
          </div>
        </div>
        <div class="grid grid-cols-3 gap-4 mt-[24px] lg:mt-[32px]">
          <div
            class="premium-card-bg rounded-[16px] p-[1px]"
          >
            <div
              class="premium-card-inner"
            >
              <h2
                class="text-[28px] md:text-[32px] lg:text-[36px] font-[700] leading-[100%]"
              >
                {{ days < 10 ? "0" + days : days }}
              </h2>
              <p
                class="text-[14px] md:text-[17px] lg:text-[18px] leading-[100%] text-[#84FFC1]"
              >
                DAYS
              </p>
            </div>
          </div>
          <div
            class="premium-card-bg rounded-[16px] p-[1px]"
          >
            <div
              class="premium-card-inner"
            >
              <h2
                class="text-[28px] md:text-[32px] lg:text-[36px] font-[700] leading-[100%]"
              >
                {{ hours < 10 ? "0" + hours : hours }}
              </h2>
              <p
                class="text-[14px] md:text-[17px] lg:text-[18px] leading-[100%] text-[#84FFC1]"
              >
                HOURS
              </p>
            </div>
          </div>
          <div
            class="premium-card-bg rounded-[16px] p-[1px]"
          >
            <div
              class="premium-card-inner"
            >
              <h2
                class="text-[28px] md:text-[32px] lg:text-[36px] font-[700] leading-[100%]"
              >
                {{ minutes < 10 ? "0" + minutes : minutes }}
              </h2>
              <p
                class="text-[14px] md:text-[17px] lg:text-[18px] leading-[100%] text-[#84FFC1]"
              >
                MINUTES
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="grid md:grid-cols-4 lg:grid-cols-7 gap-[12px] md:gap-[20px] lg:gap-[26px] md:bg-[#0B1C23]/45 rounded-[24px] md:p-[20px] md:border border-[#3D5960]">
      <img
        src="../assets/images/icons/medalion.svg"
        alt=""
        class="hidden md:block md:col-span-1 w-full md:w-[108px] md:h-[108px] lg:w-[150px] lg:h-[150px] mx-auto"
      />
      <div
        class="relative md:col-span-3 lg:col-span-2 grid grid-cols-3 gap-4 border border-[#393D41] rounded-[16px] p-[16px] bg-[#0B1C23]/45"
      >
        <p
          class="hidden md:block absolute top-0 right-0 pl-[32px] pr-[10px] py-[1px] flex items-center justify-center bg-[#84FFC1] text-black text-[16px] leading-[140%] font-[800] rounded-bl-[12px] rounded-tr-[12px]"
        >
          {{ currentYear }}
        </p>
        <div class="grid gap-[12px]">
          <h2 class="text-[22px] md:text-[28px] font-[700] leading-[110%]">
            $4.3B
          </h2>
          <p class="text-[12px] md:text-[14px] leading-[126%]">
            Startup Ecosystem Valuation
          </p>
        </div>
        <div class="grid gap-[12px]">
          <h2 class="text-[22px] md:text-[28px] font-[700] leading-[110%]">
            #1
          </h2>
          <p class="text-[12px] md:text-[14px] leading-[126%]">
            In venture investment growth globally
          </p>
        </div>
        <div class="grid gap-[48px]">
          <div class="flex md:hidden items-center justify-end">
            <p
              class="w-[51px] h-[25px] bg-[#84FFC1] text-black text-[12px] md:text-[16px] leading-[140%] font-[800] py-[4px] px-[10px] rounded-[6px]"
            >
              {{ currentYear }}
            </p>
          </div>
          <div class="flex items-center justify-end md:pt-[55px]">
            <img src="../assets/images/icons/diag.svg" alt="" class="" />
          </div>
        </div>
      </div>
      <div
        class="relative md:col-span-2 lg:col-span-2  grid grid-cols-4 md:grid-cols-3 gap-4 border border-[#393D41] rounded-[16px] p-[16px] bg-[#0B1C23]/45"
      >
        <p
  class="hidden md:block absolute top-0 right-0
         pl-[32px] pr-[10px] py-[1px]
         flex items-center justify-center
         bg-[#84FFC1] text-black
         text-[16px] leading-[140%] font-[800]
         rounded-bl-[12px] rounded-tr-[12px]"
>
  {{ currentYear }}
</p>
        <img
          src="../assets/images/icons/medalion.svg"
          alt=""
          class="py-[27px] md:hidden"
        />
        <div class="grid gap-[12px]">
          <h2 class="text-[22px] md:text-[28px] font-[700] leading-[110%]">#1</h2>
          <p class="text-[12px] md:text-[14px] leading-[126%]">
            Ecosystem in the World by Growth Rate
          </p>
        </div>
        <div class="grid gap-[12px]">
          <h2 class="text-[22px] md:text-[28px] font-[700] leading-[110%]">#1</h2>
          <p class="text-[12px] md:text-[14px] leading-[126%]">
            Startup Hub in Central Asia (Tashkent)
          </p>
        </div>
        <div class="grid gap-[56px]">
          <div class="flex md:hidden items-center justify-end">
            <p
              class="w-[51px] h-[25px] bg-[#84FFC1] text-black text-[12px] md:text-[16px] leading-[140%] font-[800] py-[4px] px-[10px] rounded-[6px]"
            >
              {{ currentYear }}
            </p>
          </div>
          <div class="flex items-center justify-end md:pt-[55px]">
            <img src="../assets/images/icons/stblink.svg" alt="" class="" />
          </div>
        </div>
      </div>
      <div
        class="relative md:col-span-2 lg:col-span-2 grid grid-cols-3 gap-4 border border-[#393D41] rounded-[16px] p-[16px] bg-[#0B1C23]/45"
      >
        <p
  class="hidden md:block absolute top-0 right-0
         pl-[32px] pr-[10px] py-[1px]
         flex items-center justify-center
         bg-[#84FFC1] text-black
         text-[16px] leading-[140%] font-[800]
         rounded-bl-[12px] rounded-tr-[12px]"
>
  {{ currentYear }}
</p>
        <div class="grid gap-[32px]">
          <h2
            class="flex items-center gap-[6px] text-[22px] md:text-[28px] font-[700] leading-[110%]"
          >
            2
            <img src="../assets/images/icons/horse.svg" alt="" />
          </h2>
          <p class="text-[12px] md:text-[14px] leading-[126%]">Fintech Unicorns</p>
        </div>
        <div class="grid gap-[12px]">
          <img src="../assets/images/icons/uzum.svg" alt="" />
          <img src="../assets/images/icons/tbc.svg" alt="" />
        </div>
        <div class="grid gap-[12px]">
          <div class="flex justify-end md:hidden">
            <p
              class="w-[51px] h-[25px] bg-[#84FFC1] text-black text-[12px] md:text-[16px] leading-[140%] font-[800] py-[4px] px-[10px] rounded-[6px]"
            >
              {{ currentYear }}
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref, onMounted, onUnmounted } from "vue";

const days = ref(0);
const hours = ref(0);
const minutes = ref(0);

const currentYear = new Date().getFullYear();

let timerId = null;

const calculateCountdown = () => {
  const targetDate = new Date("2026-11-01T00:00:00+05:00").getTime();
  const now = new Date().getTime();
  const timeDifference = targetDate - now;

  if (timeDifference <= 0) {
    days.value = 0;
    hours.value = 0;
    minutes.value = 0;
    if (timerId) clearInterval(timerId);
    return;
  }

  days.value = Math.floor(timeDifference / (1000 * 60 * 60 * 24));
  hours.value = Math.floor(
    (timeDifference % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60),
  );
  minutes.value = Math.floor((timeDifference % (1000 * 60 * 60)) / (1000 * 60));
};

onMounted(() => {
  calculateCountdown();
  timerId = setInterval(calculateCountdown, 60000);
});

onUnmounted(() => {
  if (timerId) clearInterval(timerId);
});
</script>

<style lang="scss" scoped>
.premium-card-bg {
  background:
    radial-gradient(ellipse at 15% 0%, rgba(255, 255, 255, 0.6) 0%, transparent 60%),
    radial-gradient(ellipse at 100% 15%, rgba(255, 255, 255, 0.2) 0%, transparent 0%),
    radial-gradient(ellipse at 0% 85%, rgba(255, 255, 255, 0.2) 0%, transparent 0%),
    radial-gradient(ellipse at 85% 100%, rgba(255, 255, 255, 0.4) 0%, transparent 60%),
    #0e171e;
}
.premium-card-inner {
  padding-top: 20px;
  padding-bottom: 20px;
  border-radius: 16px;
  text-align: center;
  display: grid;
  gap: 6px;
  background: #0A111A;
}
</style>
