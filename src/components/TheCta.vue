<template>
  <section class="py-[24px] md:py-0 px-[16px] md:px-[32px] lg:px-0">
    <div
      class="premium-card-bg w-full rounded-[16px] p-[16px] md:p-[20px] lg:px-[42px] lg:py-[36px] flex flex-col lg:flex-row justify-between gap-8 border border-[#3D5960] bg-[#0B1C23]/45"
    >
      <div class="w-full lg:w-[45%] flex-shrink-0 order-1 lg:order-2">
        <picture class="w-full block">
          <source
            media="(min-width: 1024px)"
            srcset="../assets/images/Catfirst.webp"
          />
          <img
            src="../assets/images/Catsecond.webp"
            alt="ICT Week Conference Stage"
            class="w-full h-[233px] md:h-auto object-cover rounded-[8px]"
            loading="lazy"
          />
        </picture>
      </div>

      <div
        class="flex flex-col justify-center gap-[24px] md:gap-5 lg:gap-[56px] text-left order-2 lg:order-1 w-full lg:self-stretch"
      >
        <h2
          class="text-[#EDEDF2] text-[26px] md:text-[36px] lg:text-[48px] font-[800] leading-[120%] tracking-tight"
        >
          Save your spot today!
        </h2>

        <div
          class="flex flex-col gap-3 text-[#B4B6B8] text-[14px] md:text-[16px] lg:text-[18px] leading-[160%] font-medium"
        >
          <p>
            Every unicorn starts as a single star. Together they become the
            Northern Lights.
          </p>
          <p>
            Welcome to Uzbekistan, where visionary government support and a
            thriving innovation ecosystem help founders turn bold ideas into
            global ventures.
          </p>
          <p>
            Here, startups and tech companies don't just become part of the
            Northern Lights—they discover their North Star and follow it all the
            way to international success.
          </p>
        </div>

        <div class="mt-2">
          <button
            type="button"
            @click="
              document
                .getElementById('register')
                ?.scrollIntoView({ behavior: 'smooth' })
            "
            class="w-full h-[48px] md:w-[190px] md:h-[54px] px-[24px] rounded-[12px] bg-[#77EAB0] text-[#0A1614] font-[700] text-[16px] lg:text-[18px] leading-[24px] flex items-center justify-center gap-[10px] hover:brightness-110 active:scale-98 transition duration-200 cursor-pointer border-0 outline-none"
          >
            <span>Register now ↗</span>
          </button>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup></script>

<style lang="scss" scoped></style>
