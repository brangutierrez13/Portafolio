<template>
  <section class="w-full lg:h-screen h-[180vh] grid lg:grid-cols-2 grid-cols-1">
    <article
      class="flex flex-col md:px-20 pt-32 px-5 animate__animated animate__fadeInLeft"
    >
      <div class="text-7xl font-bold">
        Mis Skills como <span class="text-red-500">FrontEnd</span>
      </div>
      <div class="mt-10 mb-5 text-2xl font-light">
        Te contare sobre mis habilidades como desarrollador FrontEnd Web y
        algunas experiencias.
      </div>
      <SocialLinks />
    </article>
    <article class="flex flex-row lg:items-center justify-center">
      <NuxtImg src="/icons/code.svg"></NuxtImg>
    </article>
  </section>
  <section class="w-full h-screen flex flex-col px-20">
    <div class="text-7xl font-bold mb-10">
      Habilidades <span class="text-red-500">adquiridas</span>
    </div>
    <div class="text-6xl font-bold">Esenciales en el FrontEnd</div>
    <article class="w-full h-full mt-10">
      <div
        v-for="(item, index) in esentials"
        :key="index"
        class="flex flex-row"
      >
        <NuxtImg class="size-[100px]" :src="item.image"></NuxtImg>

        <div class="text-2xl font-light ml-10">
          {{ item.text }}
        </div>
      </div>
    </article>
  </section>
  <section class="w-full h-screen flex flex-col px-20">

  </section>
</template>

<script>
export default {
  data: () => ({
    esentials: [
      {
        index: 1,
        image: "/icons/html.png",
        text: "Tengo habilidades sobre la maquetacion a traves de codigo HTML, utilizando la mayoria de etiquetas con la finalidad de que la pagina web sea lo mas semantico posible.",
      },
      {
        index: 2,
        image: "/icons/css.png",
        text: "No puedo olvidarme de CSS para estilzar todo lo construido con HTML, aplicando estilos unicos y atractivos a traves de este mismo, ya sea utilizando archivo .CSS o inscrustando <style> en los HTML.",
      },
      {
        index: 3,
        image: "/icons/js.png",
        text: "No puede faltar los scripts que se puedan ocupar en HTML, aplicando funcionalidades que se requieran en el desarrollo de una pagina web.",
      },
    ],
  }),
};
</script>
