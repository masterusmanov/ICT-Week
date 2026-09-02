<template>
  <header
    class="relative w-full md:max-w-[720px] lg:max-w-[1040px] h-[80px] mx-auto md:rounded-full md:mt-[37px] md:p-[2px] lg:px-[3px]"
    style="
      background:
        radial-gradient(
          ellipse at 15% 0%,
          rgba(255, 255, 255, 0.6) 0%,
          transparent 40%
        ),
        radial-gradient(
          ellipse at 100% 15%,
          rgba(255, 255, 255, 0.2) 0%,
          transparent 0%
        ),
        radial-gradient(
          ellipse at 0% 85%,
          rgba(255, 255, 255, 0.2) 0%,
          transparent 0%
        ),
        radial-gradient(
          ellipse at 85% 100%,
          rgba(255, 255, 255, 0.4) 0%,
          transparent 40%
        ),
        #0e171e;
    "
  >
    <div
      class="w-full h-full flex items-center justify-between bg-[#1A2B2C]/85 md:rounded-full px-[18px] md:pl-[20px] lg:pr-[14px] lg:pl-[32px] select-none gap-2"
    >
      <div class="flex items-center flex-shrink-0 md:ml-[32px] lg:ml-0">
        <img
          src="../assets/images/CompLogo.svg"
          alt="ICT WEEK Logo"
          class="w-[56.57px] h-[36px] md:w-[57.43px] md:h-[36px] lg:w-[67px] lg:h-[42px]"
        />
      </div>

      <nav class="header__nav hidden md:block flex-1 max-w-[384px] mx-4">
        <ul
          class="w-full h-[52px] flex items-center justify-between rounded-full px-[6px] gap-[16px] lg:gap-2"
        >
          <li class="h-[40px] flex items-center flex-1 max-w-[100px]">
            <a
              href="#app"
              class="w-full h-full flex items-center justify-center bg-gradient-to-b from-[#142C28] to-[#0A1614] border border-[#1E463F]/50 text-white rounded-full text-[14px] lg:text-[16px] font-semibold shadow-[0_4px_12px_rgba(0,0,0,0.4)] transition-all duration-200 select-none"
            >
              Home
            </a>
          </li>
          <li class="flex-1 text-center">
            <a
              href="#program"
              class="text-white/60 hover:text-white text-[12px] leading-[140%] lg:text-[16px] font-medium transition-all duration-200 select-none block"
              >Program</a
            >
          </li>
          <li class="flex-1 text-center">
            <a
              href="#partners"
              class="text-white/60 hover:text-white text-[12px] leading-[140%] lg:text-[16px] font-medium transition-all duration-200 select-none block"
              >Partners</a
            >
          </li>
          <li class="flex-1 text-center">
            <a
              href="#incentives"
              class="text-white/60 hover:text-white text-[12px] leading-[140%] lg:text-[16px] font-medium transition-all duration-200 select-none block"
              >Incentives</a
            >
          </li>
        </ul>
      </nav>

      <div class="flex items-center gap-[12px] flex-shrink-0">
        <div
          class="lang-dropdown hidden md:block md:w-[81px] md:h-[36px] lg:w-[119px] lg:h-[52px] rounded-full p-[2px]"
          style="
            background:
              radial-gradient(
                ellipse at 15% 0%,
                rgba(255, 255, 255, 0.6) 0%,
                transparent 40%
              ),
              radial-gradient(
                ellipse at 100% 15%,
                rgba(255, 255, 255, 0.2) 0%,
                transparent 5%
              ),
              radial-gradient(
                ellipse at 0% 85%,
                rgba(255, 255, 255, 0.2) 0%,
                transparent 5%
              ),
              radial-gradient(
                ellipse at 85% 100%,
                rgba(255, 255, 255, 0.4) 0%,
                transparent 40%
              ),
              #0e171e;
          "
        >
          <div class="relative w-full h-full">
            <button
              type="button"
              @click="isOpen = !isOpen"
              class="w-full h-full flex items-center gap-[4px] md:justify-center text-[#B5B2B1] lg:justify-between bg-[#0E171E] hover:bg-[#14202A] md:pl-[14px] lg:pl-[14px] pr-[16px] rounded-full md:text-[12px] lg:text-[16px] font-medium transition cursor-pointer select-none border-0 outline-none"
            >
              <span>{{ currentLang }}</span>
              <img
                src="../assets/images/icons/arrow-down.webp"
                alt="Arrow"
                class="w-3 h-3 opacity-70 transition-transform duration-200"
                :class="{ 'rotate-180': isOpen }"
              />
            </button>

            <transition
              enter-active-class="transition duration-100 ease-out"
              enter-from-class="transform scale-95 opacity-0"
              enter-to-class="transform scale-100 opacity-100"
              leave-active-class="transition duration-75 ease-in"
              leave-from-class="transform scale-100 opacity-100"
              leave-to-class="transform scale-95 opacity-0"
            >
              <div
                v-if="isOpen"
                class="absolute right-0 mt-2 w-36 bg-[#0E171E] border border-white/10 rounded-2xl p-1.5 shadow-2xl z-50 backdrop-blur-xl"
              >
                <button
                  type="button"
                  v-for="lang in languages"
                  :key="lang"
                  @click="changeLanguage(lang)"
                  class="w-full text-left px-4 py-2 rounded-xl text-sm transition cursor-pointer text-white/70 hover:bg-white/5 hover:text-white"
                  :class="{
                    'bg-gradient-to-r from-[#62ECC4]/20 to-[#2FD398]/10 text-[#62ECC4] font-medium':
                      currentLang === lang,
                  }"
                >
                  {{ lang }}
                </button>
              </div>
            </transition>
          </div>
        </div>

        <button
          @click="scrollToRegister"
          class="h-[38px] md:h-[36px] lg:h-[52px] px-[16px] py-[10px] md:px-[12px] md:py-[10px] lg:px-[24px] lg:py-[15px] flex items-center justify-center gap-[10px] text-[#121B26] rounded-full bg-gradient-to-b from-[#84FFC1] to-[#459B6F] font-semibold text-[13px] md:text-[12px] lg:text-[16px] transition-all duration-200 hover:brightness-110 active:scale-98 cursor-pointer select-none border-0 outline-none"
          type="button"
        >
          Register Now
        </button>
        <button
          class="md:hidden w-[40px] h-[40px] rounded-[8px] bg-[#424B51] flex items-center justify-center cursor-pointer select-none"
          type="button"
          :aria-expanded="isMobileMenuOpen"
          :aria-label="
            isMobileMenuOpen ? 'Close mobile menu' : 'Open mobile menu'
          "
          @click="isMobileMenuOpen = !isMobileMenuOpen"
        >
          <div class="grid grid-cols-1 gap-[4px]">
            <div
              class="bg-white w-[20px] h-[3px] rounded-full transition-transform duration-200"
              :class="{ 'rotate-45 translate-y-[7px]': isMobileMenuOpen }"
            ></div>
            <div
              class="bg-white w-[20px] h-[3px] rounded-full transition-opacity duration-200"
              :class="{ 'opacity-0': isMobileMenuOpen }"
            ></div>
            <div
              class="bg-white w-[20px] h-[3px] rounded-full transition-transform duration-200"
              :class="{ '-rotate-45 -translate-y-[7px]': isMobileMenuOpen }"
            ></div>
          </div>
        </button>

        <transition
          enter-active-class="transition duration-200 ease-out"
          enter-from-class="transform -translate-y-5 opacity-0"
          enter-to-class="transform translate-y-0 opacity-100"
          leave-active-class="transition duration-150 ease-in"
          leave-from-class="transform translate-y-0 opacity-100"
          leave-to-class="transform -translate-y-5 opacity-0"
        >
          <div
            v-if="isMobileMenuOpen"
            class="absolute top-[90px] left-0 w-full bg-[#0E171E]/95 backdrop-blur-xl border border-white/10 rounded-[24px] p-6 z-40 flex flex-col gap-6 shadow-2xl"
          >
            <nav>
              <ul class="flex flex-col gap-4 text-center">
                <li>
                  <a
                    href="#app"
                    @click="isMobileMenuOpen = false"
                    class="block py-2 text-white bg-gradient-to-b from-[#142C28] to-[#0A1614] border border-[#1E463F]/50 rounded-full font-semibold text-[16px]"
                  >
                    Home
                  </a>
                </li>
                <li>
                  <a
                    href="#program"
                    @click="isMobileMenuOpen = false"
                    class="block py-2 text-white/70 hover:text-white text-[16px] font-medium transition"
                    >Program</a
                  >
                </li>
                <li>
                  <a
                    href="#partners"
                    @click="isMobileMenuOpen = false"
                    class="block py-2 text-white/70 hover:text-white text-[16px] font-medium transition"
                    >Partners</a
                  >
                </li>
                <li>
                  <a
                    href="#incentives"
                    @click="isMobileMenuOpen = false"
                    class="block py-2 text-white/70 hover:text-white text-[16px] font-medium transition"
                    >Incentives</a
                  >
                </li>
              </ul>
            </nav>

            <div class="w-full h-[1px] bg-white/10"></div>

            <div class="flex flex-col gap-4 items-center">
              <div class="relative w-full max-w-[200px]">
                <button
                  type="button"
                  @click.stop="isOpen = !isOpen"
                  class="w-full h-[48px] flex items-center justify-between bg-[#1A2B2C] text-white px-5 rounded-full text-[16px] font-medium border border-white/10"
                >
                  <span>{{ currentLang }}</span>
                  <img
                    src="../assets/images/icons/arrow-down.webp"
                    alt="Arrow"
                    class="w-3 h-3 opacity-70 transition-transform"
                    :class="{ 'rotate-180': isOpen }"
                  />
                </button>

                <div
                  v-if="isOpen"
                  @click.stop
                  class="absolute left-0 right-0 mt-2 bg-[#0E171E] border border-white/10 rounded-xl p-1 z-50"
                >
                  <button
                    v-for="lang in languages"
                    :key="lang"
                    @click="
                      changeLanguage(lang);
                      isMobileMenuOpen = false;
                    "
                    class="w-full text-left px-4 py-2 text-sm text-white/70 hover:bg-white/5 rounded-lg"
                  >
                    {{ lang }}
                  </button>
                </div>
              </div>
            </div>
          </div>
        </transition>
      </div>
    </div>
  </header>
</template>

<script setup>
import { ref, onMounted, onUnmounted } from "vue";

const isOpen = ref(false);
const currentLang = ref("English");
const languages = ["English", "O'zbekcha", "Русский"];

const isMobileMenuOpen = ref(false);

const changeLanguage = (lang) => {
  currentLang.value = lang;
  isOpen.value = false;
};

const scrollToRegister = () => {
  document.getElementById("register")?.scrollIntoView({ behavior: "smooth" });
  isMobileMenuOpen.value = false;
};

const closeDropdown = (e) => {
  if (!e.target.closest(".lang-dropdown")) {
    isOpen.value = false;
  }
};

onMounted(() => window.addEventListener("click", closeDropdown));
onUnmounted(() => window.removeEventListener("click", closeDropdown));
</script>

<style lang="scss" scoped></style>
