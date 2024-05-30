import Toast from 'vue-toastification'; import { useToast } from
'vue-toastification'; import VueToastificationPlugin from 'vue-toastification';
<template>
  <section
    class="w-full xl:h-[120vh] h-[180-vh] flex lg:flex-row flex-col lg:items-start items-center relative overflow-hidden"
  >
    <article
      class="flex flex-col md:px-20 pt-32 px-5 lg:w-[50%] animate__animated animate__fadeInLeft"
    >
      <div class="text-7xl font-bold">
        Soy <span class="text-red-500">FrontEnd</span> Developer
      </div>
      <div class="mt-2 font-light text-3xl">Brandon Gutierrez Jimenez</div>
      <div class="my-5 text-2xl font-light">
        Me gusta la tecnologia, desarrollar propuestas atractivas y funcionales.
        Soy Brandon Gutierrez Jimenez - Soy desarrollador
        <span class="text-red-500 font-semibold">Front-End</span>
      </div>
      <SocialLinks />
      <CustomButton
        download
        :customClass="'w-[200px] h-[50px] bg-red-500 text-white mt-10 font-semibold hover:scale-110 duration-200'"
        :icon="'bi bi-file-earmark-text-fill'"
        :text="'Descargar CV'"
        :link="'/docs/CV.pdf'"
        @click="getCV"
      ></CustomButton>
    </article>
    <NuxtImg
      class="size-[700px] xl:absolute right-[-1rem] top-[3rem] animate__animated animate__fadeIn"
      src="/blobs/blob.svg"
    />
    <NuxtImg
      class="absolute w-[700px] xl:right-[4rem] xl:bottom-[-15rem] md:bottom-[-24rem] md:right-[1rem] bottom-0 animate__animated animate__fadeInUp"
      src="/Rectangle.png"
    />
  </section>
</template>
<script>
export default {
  data: () => ({}),

  methods: {
    async getCV() {
      try {
        this.$toast.success(
          "Se ha descargado el CV.",
          {
            position: "top-center",
          },
          {
            containerClassName: "my-container-class",
          }
        );
      } catch (error) {}
    },
  },
};
</script>