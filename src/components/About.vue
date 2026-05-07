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
      threshold: 0.4,
    },
  );

  const section = document.querySelector("#about");

  if (section) {
    observer.observe(section);
  }
});
</script>
<template>
  <section
    id="about"
    class="min-h-screen relative flex items-center justify-center px-6 md:px-16 py-[120px]"
  >
    <img
      src="/public/images/pattern4.webp"
      alt=""
      class="w-40 md:w-40 absolute -left-1 md:-left-1 top-5 md:top-2 opacity-80 scale-x-[-1]"
    />
    <div
      :class="show ? 'opacity-100 translate-y-0' : 'opacity-0 translate-y-20'"
      class="bg-gray-50 border-4 border-gray-800 rounded-3xl p-8 md:p-10 shadow-[10px_10px_0px_gray] transition-all duration-700 ease-out"
    >
      <!-- LABEL -->
      <p
        class="inline-block bg-gray-900 rounded-2xl text-white px-4 py-2 font-black mb-5"
      >
        ABOUT ME
      </p>

      <!-- TITLE -->
      <h1 class="text-4xl md:text-6xl font-black leading-tight mb-6">
        Frontend Developer <br />
        & Creative Designer
      </h1>

      <!-- DESC -->
      <p
        class="font-bold text-gray-700 leading-relaxed mb-6 w-full md:w-3/4 text-lg"
      >
        Saya adalah seorang frontend enthusiast yang suka membangun website
        modern, interaktif, dan responsive menggunakan Vue JS, Laravel, dan
        Tailwind CSS.
      </p>
      <!-- SKILLS -->
      <div class="flex flex-wrap gap-4">
        <div
          class="bg-yellow-300 border-4 border-gray-800 px-5 py-3 font-black shadow-[4px_4px_0px_gray]"
        >
          Vue JS
        </div>

        <div
          class="bg-green-300 border-4 border-gray-800 px-5 py-3 font-black shadow-[4px_4px_0px_gray]"
        >
          HTML & CSS
        </div>

        <div
          class="bg-blue-300 border-4 border-gray-800 px-5 py-3 font-black shadow-[4px_4px_0px_gray]"
        >
          Tailwind
        </div>

        <div
          class="bg-pink-300 border-4 border-gray-800 px-5 py-3 font-black shadow-[4px_4px_0px_gray]"
        >
          UI/UX
        </div>
      </div>
    </div>
  </section>
</template>
