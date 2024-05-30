
<template>
  <section class="w-full lg:h-screen h-[180vh] grid lg:grid-cols-2 grid-cols-1">
    <article
      class="flex flex-col md:px-20 pt-32 px-5 animate__animated animate__fadeInLeft"
    >
      <div class="text-7xl font-bold">
        Mi <span class="text-red-500">historia</span> Quien soy?
      </div>
      <div class="mt-10 mb-5 text-2xl font-light">
        Te contare un poco de mi historia como desarrollador de Front-End y de
        mas.
      </div>
      <SocialLinks />
    </article>
    <article class="flex flex-row lg:items-center justify-center">
        <NuxtImg src="/photo.jpg" class="rounded-[50%] size-[400px] border-[5px] border-solid border-red-500"></NuxtImg>
    </article>
  </section>
  <section class="w-full lg:h-screen h-[180vh] grid lg:grid-cols-2 grid-cols-1">
    <article class="flex flex-row justify-center p-0 m-0">
        <NuxtImg class="lg:size-[auto] size-[500px]" src="/blobs/Shape.png"></NuxtImg>
    </article>
    <article class="md:p-20 px-5">
        <div class="text-4xl font-bold">Mi nombre es <span class="text-red-500">Brandon Gutierrez Jimenez</span></div>
        <div class="text-2xl font-light mt-10">Soy egresado de la Universidad Tecnologica de Tecamachalco como <span>Ingeniero e Desarrollo y Gestion de Software</span>, en la region de Tecamachalco de Guerreo, Puebla.
Tengo 23 anios y siempre me ha gustado la tecnologia.</div>
    </article>
  </section>
  <section class="w-full lg:h-screen h-[180vh] grid lg:grid-cols-2 grid-cols-1 md:p-20 px-5">
    <article>
        <div class="text-5xl font-bold">Estudie en <span class="text-red-500">Universidad Tecnologica de Tecamachalco</span></div>
        <div class="text-2xl font-light mt-10">
            La Universidad Tecnológica de Tecamachalco (UTT) es una institución educativa ubicada en Tecamachalco de Guerrero, Puebla, México. 
        </div>
    </article>
    <article>
        <NuxtImg src="/utt.png"></NuxtImg>
    </article>
  </section>
</template>
