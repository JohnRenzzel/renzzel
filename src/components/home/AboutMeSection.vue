<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'ExperienceSection'
})
</script>

<template>
  <section
    id="about-me-section"
    class="wrapper flex flex-col md:flex-row items-center md:items-start py-12 md:py-24"
  >
    <div class="mb-8 md:mb-0" data-aos="fade-right" data-aos-duration="1000">
      <div class="img-animation w-64 mb-2 md:mb-4">
        <img
          src="./../../assets/img/home/about_me/john.jpg"
          alt="Zdjęcie profilowe"
          width="300"
          height="300"
        />
      </div>
      <div class="flex flex-col items-center">
        <p class="text-center mx-4">Future Developer</p>
        <p class="text-center mx-4"><strong>John Renzzel</strong></p>
      </div>
    </div>
    <div class="mx-4 md:ms-8" data-aos="fade-left" data-aos-duration="1000">
      <h2 class="text-center md:text-left text-3xl md:text-4xl mb-4">John Ronald Tajanlangit</h2>
      <p class="text-justify md:text-left mb-2">
        Hello! I'm a passionate Web Development student with a drive for building user-centric and
        efficient websites and applications. Currently pursuing a degree in BSIT at
        <strong>Cordova Public College</strong>, I am eagerly diving into the world of coding,
        design, and technology innovation.
      </p>
      <p class="text-justify md:text-left mb-2">
        Outside of web development, I have a profound interest in the world of online gaming,
        particularly within the emerging NFT space, where the blend of technology and gaming creates
        a unique and engaging experience. Games like
        <strong>Pixels, Mavia and Nightcrows</strong> not only offer entertainment but also provide
        a fascinating insight into the application of blockchain technology and digital ownership in
        virtual environments.
      </p>
      <p class="text-justify md:text-left mb-2">
        These interests not only serve as a leisure activity but also inspire my approach to web
        development, encouraging me to think critically and creatively in both coding and design.
      </p>
    </div>
  </section>
</template>

<style scoped>
.img-animation {
  padding: 8px;
  --border-size: 5px;
  --border-angle: 0turn;
  background-image: conic-gradient(
      from var(--border-angle),
      rgb(255, 255, 255),
      rgb(255, 255, 255) 50%,
      rgb(255, 255, 255)
    ),
    conic-gradient(from var(--border-angle), transparent 20%, #9333ea, #222222);
  background-size:
    calc(100% - var(--border-size) * 2) calc(100% - var(--border-size) * 2),
    cover;
  background-position: center center;
  background-repeat: no-repeat;
  animation: bg-spin 3s linear infinite;
}
@property --border-angle {
  syntax: '<angle>';
  inherits: true;
  initial-value: 0turn;
}
@keyframes bg-spin {
  to {
    --border-angle: 1turn;
  }
}
</style>
