import { NuxtLink } from '../.nuxt/components';
<template>
  <header class="w-full h-[80px] fixed z-50 bg-white">
    <nav
      class="flex flex-row xl:px-20 px-5 w-full h-full items-center justify-between"
    >
      <NuxtLink to="/">
        <div class="flex flex-row cursor-pointer items-center">
          <NuxtImg class="rounded-[50%] size-[50px] border-solid border-red-500 border" src="/photo.jpg" />
          <h1 class="ml-5 font-bold text-xl">Inicio</h1>
        </div>
      </NuxtLink>
      <div class="md:block hidden">
        <ul class="flex flex-row flex-wrap gap-10">
          <li
            v-for="(item, i) in Links"
            :key="i"
            class="font-light text-xl cursor-pointer hover:scale-110 duration-100 hover:text-red-500"
          >
            <NuxtLink :to="item.route">{{ item.name }}</NuxtLink>
          </li>
        </ul>
      </div>
    </nav>
  </header>
</template>

<script>
export default {
  data: () => ({
    Links: [
      {
        name: "Quien soy",
        route: "/about",
      },
      {
        name: "Skills",
        route: "/skills",
      },
      {
        name: "Experiencias y Portafolio",
        route: "/experiences",
      },
    ],
  }),
};
</script>
