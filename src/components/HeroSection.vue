<script setup>
import { ref, onMounted } from "vue";

const show = ref(false);

onMounted(() => {
  const observer = new IntersectionObserver(
    ([entry]) => {
      if (entry.isIntersecting) {
        show.value = true;
      }
    },
    {
      threshold: 0.2,
    },
  );

  const section = document.querySelector("#home");

  if (section) {
    observer.observe(section);
  }
});
</script>
<template>
  <section
    id="home"
    :class="show ? 'opacity-100 translate-y-0' : 'opacity-0 translate-y-20'"
    class="min-h-screen flex items-center justify-center px-2 sm:px-6 md:px-16 py-22 transition-all duration-700 ease-out"
  >
    <div class="max-w-7xl w-full grid md:grid-cols-2 gap-12 items-center">
      <!-- TEXT -->
      <div class="rounded-3xl p-8 md:p-12">
        <p
          class="inline-block bg-gray-900 text-white px-4 py-2 rounded-xl text-sm md:text-base font-black mb-6"
        >
          FRONTEND ENTHUSIAST
        </p>

        <h1
          class="text-5xl md:text-7xl font-black text-black leading-tight mb-2"
        >
          HI! I'M
          <span class="text-orange-500">BAYU ARDIANSYAH</span>
        </h1>

        <p class="text-lg md:text-1xl font-bold text-black mb-8">
          Saya seorang frontend developer yang fokus membangun website modern,
          responsive, dan interaktif menggunakan Vue JS & Laravel.
        </p>

        <div
          class="flex flex-row flex-wrap md:justify-start gap-4 w-full"
        >
          <!-- BUTTON PROJECT -->
          <a
            href="#projects"
            class="bg-white border-4 border-gray-900 px-5 md:px-6 py-3 font-black text-sm md:text-base shadow-[5px_5px_0px_gray] hover:translate-x-1 hover:translate-y-1 hover:shadow-none transition duration-200"
          >
            My Projects
          </a>

          <!-- BUTTON CONTACT -->
          <a
            href="#contact"
            class="bg-orange-500 text-white border-4 border-gray-900 px-5 md:px-6 py-3 font-black text-sm md:text-base shadow-[5px_5px_0px_gray] hover:translate-x-1 hover:translate-y-1 hover:shadow-none transition duration-200"
          >
            Contact Me
          </a>
        </div>
      </div>

      <!-- IMAGE -->
      <div class="hidden md:flex justify-center">
        <div
          class="bg-orange-500 border-4 border-gray-900 rounded-2xl p-2 shadow-[10px_10px_0px_gray] -rotate-2 floating"
        >
          <img
            src="/public/images/hero-image.webp"
            alt="profile"
            class="w-[280px] md:w-[310px] rounded-2xl border-4 border-black object-cover"
          />
        </div>
      </div>
    </div>
  </section>
</template>
