<script setup lang="ts">
interface Link {
  href: string
  label: string
}

const logo = "/img/full-logo.png";
const links: Link[] = [...Array(4).keys()].map(i => ({
  href: "#",
  label: `Link ${i + 1}`
}))
</script>

<template>
  <div class="absolute z-10 w-screen px-6 py-6 flex md:grid md:grid-cols-2 justify-between items-center">
    <div class="flex items-center">
      <img :src="logo" alt="SMK Negeri 7 Samarinda" class="max-h-12">
    </div>
    <nav class="hidden uppercase text-white md:flex">
      <a v-for="link in links" class="grow py-6 transition hover:scale-105" :href="link.href">{{ link.label }}</a>
    </nav>
    <button class="border rounded-lg px-4 py-3 flex flex-col gap-y-1 justify-center transition group hover:bg-white active:bg-slate-200 md:hidden">
      <div class="bg-white h-[2px] w-4 rounded group-hover:bg-primary"></div>
      <div class="bg-white h-[2px] w-4 rounded group-hover:bg-primary"></div>
      <div class="bg-white h-[2px] w-4 rounded group-hover:bg-primary"></div>
    </button>
  </div>
</template>