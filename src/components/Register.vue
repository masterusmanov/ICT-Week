<template>
    <section  class="lg:my-[48px] py-[24px] md:py-0 px-[16px]  md:px-[32px] lg:px-0">
    <div
      class="premium-card-bg text-[#EDEDF2] w-full rounded-[16px] p-[16px] md:p-[20px] lg:px-[42px] lg:py-[36px]  border border-[#3D5960] bg-[#0B1C23]/45">
       <h2 class="font-[700] text-[26px] md:text-[36px] lg:text-[56px] leading-[120%] my-[20px] md:my-[24px] lg:my-[32px] text-center">Register for ICTWEEK Uzbekistan 2026</h2>
       <p class="md:w-[70%] mx-auto text-[14px] lg:text-[20px] leading-[120%] text-center">Join global tech leaders, enterprise delegates, and investors in Tashkent. Complete your details below to secure your pass.</p>
    <div class=" px-6 py-14 bg-[#09151D] text-white">

    <div class="grid md:grid-cols-2 gap-x-8 gap-y-6">

      <div>
        <label class="block text-sm mb-2">Full name</label>
        <input type="text" placeholder="John Doe"
          class="w-full rounded-lg px-4 py-2.5 text-sm text-white placeholder-white/30 bg-white/[0.03] border border-white/10 focus:outline-none focus:border-emerald-400/50 focus:ring-2 focus:ring-emerald-400/20 transition" />
      </div>

      <div class="relative">
        <label class="block text-sm mb-2">Country</label>
        <button type="button"
          class="w-full rounded-lg px-4 py-2.5 text-sm text-left flex items-center justify-between bg-white/[0.03] border border-white/10 text-white/30">
          <span>Select Country...</span>
          <svg class="w-4 h-4 text-white/40" viewBox="0 0 20 20" fill="none"><path d="M5 7.5L10 12.5L15 7.5" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/></svg>
        </button>
      </div>

      <div>
        <label class="block text-sm mb-2">Email</label>
        <input type="email" placeholder="alex@company.com"
          class="w-full rounded-lg px-4 py-2.5 text-sm text-white placeholder-white/30 bg-white/[0.03] border border-white/10 focus:outline-none focus:border-emerald-400/50 focus:ring-2 focus:ring-emerald-400/20 transition" />
      </div>

      <div>
        <label class="block text-sm mb-2">Phone number</label>
        <input type="tel" placeholder="+998 90 123-45-67"
          class="w-full rounded-lg px-4 py-2.5 text-sm text-white placeholder-white/30 bg-white/[0.03] border border-white/10 focus:outline-none focus:border-emerald-400/50 focus:ring-2 focus:ring-emerald-400/20 transition" />
      </div>

      <div>
        <label class="block text-sm mb-2">Company</label>
        <input type="text" placeholder="Company"
          class="w-full rounded-lg px-4 py-2.5 text-sm text-white placeholder-white/30 bg-white/[0.03] border border-white/10 focus:outline-none focus:border-emerald-400/50 focus:ring-2 focus:ring-emerald-400/20 transition" />
      </div>

      <div>
        <label class="block text-sm mb-2">Position</label>
        <input type="text" placeholder="Managing Director"
          class="w-full rounded-lg px-4 py-2.5 text-sm text-white placeholder-white/30 bg-white/[0.03] border border-white/10 focus:outline-none focus:border-emerald-400/50 focus:ring-2 focus:ring-emerald-400/20 transition" />
      </div>

      <div class="relative">
        <label class="block text-sm mb-2">I am attending as</label>
        <button type="button"
          class="w-full rounded-lg px-4 py-2.5 text-sm text-left flex items-center justify-between bg-white/[0.03] border border-white/10 text-white/30">
          <span>Select category...</span>
          <svg class="w-4 h-4 text-white/40" viewBox="0 0 20 20" fill="none"><path d="M5 7.5L10 12.5L15 7.5" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/></svg>
        </button>
      </div>

      <div class="relative">
        <label class="block text-sm mb-2"> Event track(s) you plan to attend (Select all that apply)</label>
        <button type="button"
          class="w-full rounded-lg px-4 py-2.5 text-sm text-left flex items-center justify-between bg-white/[0.03] border border-white/10 text-white/30">
          <span>Select track(s)...</span>
          <svg class="w-4 h-4 text-white/40" viewBox="0 0 20 20" fill="none"><path d="M5 7.5L10 12.5L15 7.5" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/></svg>
        </button>
      </div>

      <div class="relative">
        <label class="block text-sm mb-2">BHow did you hear about us?</label>
        <button type="button"
          class="w-full rounded-lg px-4 py-2.5 text-sm text-left flex items-center justify-between bg-white/[0.03] border border-white/10 text-white">
          <span>Select source...</span>
          <svg class="w-4 h-4 text-white/40 rotate-180" viewBox="0 0 20 20" fill="none"><path d="M5 7.5L10 12.5L15 7.5" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/></svg>
        </button>

        <div class="absolute z-10 mt-2 w-full rounded-lg bg-[#0b1512] border border-white/10 shadow-xl overflow-hidden">
          <div class="px-4 py-2.5 text-sm hover:bg-white/5 cursor-pointer flex items-center gap-2">
            <span class="w-3.5 h-3.5 rounded-full border border-white/30 flex-shrink-0"></span>
            Onlayn Advertisement (Instagram, Facebook, LinkedIn, Google)
          </div>
          <div class="px-4 py-2.5 text-sm hover:bg-white/5 cursor-pointer flex items-center gap-2">
            <span class="w-3.5 h-3.5 rounded-full border border-emerald-400 bg-emerald-400 flex-shrink-0"></span>
            Partner Network
          </div>
          <div class="px-4 py-2.5 text-sm hover:bg-white/5 cursor-pointer flex items-center gap-2">
            <span class="w-3.5 h-3.5 rounded-full border border-white/30 flex-shrink-0"></span>
            IT Park Representative
          </div>
          <div class="px-4 py-2.5 text-sm hover:bg-white/5 cursor-pointer flex items-center gap-2">
            <span class="w-3.5 h-3.5 rounded-full border border-white/30 flex-shrink-0"></span>
            Organic Search / Website
          </div>
        </div>
      </div>

      <div>
        <label class="block text-sm mb-2">Name of focal point in IT Park (if available)</label>
        <input type="text" placeholder="e.g. Contact person or team member name"
          class="w-full rounded-lg px-4 py-2.5 text-sm text-white placeholder-white/30 bg-white/[0.03] border border-white/10 focus:outline-none focus:border-emerald-400/50 focus:ring-2 focus:ring-emerald-400/20 transition" />
      </div>
    </div>

   
    <div class="mt-10 flex flex-col md:flex-row md:items-center md:justify-between gap-6">
      <label class="flex items-start gap-2.5 text-sm text-white/50 max-w-lg cursor-pointer">
        <input type="checkbox"
          class="mt-0.5 w-4 h-4 rounded border border-white/25 bg-transparent flex-shrink-0 accent-emerald-400" />
      </label>
       <button
                class="p-[12px] flex items-center gap-1 border border-[#62ECC4] text-[#62ECC4] hover:bg-[#62ECC4] hover:text-black font-semibold rounded-[12px] text-[16px] lg:text-[18px]"
              >
                Register now ↗
              </button>
    </div>
  </div>    
    
    </div>
    </section>
</template>

<script setup>

</script>

<style lang="scss" scoped>

</style>