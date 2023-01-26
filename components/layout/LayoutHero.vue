<script setup lang="ts">
const bgImg = '/img/hero-background.png';
const heroImg = '/img/hero-img.png';
</script>

<template>

  <section id="hero" class="bg-cover bg-center" 
    :style="{ backgroundImage: `url('${bgImg}')`}"
  >
    <div class="bg-primary/80 text-white px-8 h-96 flex">
      <img :src="heroImg" alt="Selamat Datang" 
        class="hidden h-full md:block"
      >
      <div class="flex flex-col justify-center">
        <h1 id="hero-title" class="text-3xl font-extrabold uppercase pb-4">Selamat <span class="text-secondary">Datang</span></h1>
        <p class="text-sm">
          SMK Negeri 7 Samarinda sebagai <span class="font-bold uppercase">SMK Pusat Keunggulan</span> yang menghasilkan sumber daya manusia bermutu dan berdaya saing tinggi menuju <span class="font-bold uppercase">Center Of Excellency</span>.
        </p>
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