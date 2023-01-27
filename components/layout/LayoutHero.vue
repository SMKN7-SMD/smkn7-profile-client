<script setup lang="ts">
const bgImg = '/img/hero-background.png';
const heroImg = '/img/hero-img.png';
</script>

<template>
  <section id="hero" class="bg-cover bg-center relative" :style="{ backgroundImage: `url('${bgImg}')`}">
    <div class="bg-primary/80 absolute inset-0"></div>
    <div class="text-white h-[45vh] max-w-7xl px-8 mx-auto flex items-end overflow-hidden relative md:pl-0 lg:h-[55vh]">
      <img :src="heroImg" alt="Selamat Datang"
        class="hidden max-h-[20rem] md:block lg:max-h-[24rem] xl:max-h-[28rem]"
      >
      <div class="flex flex-col grow justify-center items-start h-full">
        <h1 id="hero-title" class="text-4xl font-extrabold uppercase pb-4 lg:text-5xl">
          Selamat <span class="text-secondary">Datang</span>
        </h1>
        <p class="text-sm leading-6 mb-6">
          SMK Negeri 7 Samarinda sebagai <span class="font-bold uppercase">SMK Pusat Keunggulan</span> yang menghasilkan sumber daya manusia bermutu dan berdaya saing tinggi menuju <span class="font-bold uppercase">Center Of Excellency</span>.
        </p>
        <a href="#" class="uppercase border-2 border-white font-bold rounded-md px-8 py-3 transition hover:bg-white hover:text-primary">
          Jelajahi
        </a>
      </div>
    </div>
  </section>
</template>

<style>
#hero-title {
  text-shadow: 0px 1px, 1px 0px, 1px 1px;
  letter-spacing: 2px;
}
</style>