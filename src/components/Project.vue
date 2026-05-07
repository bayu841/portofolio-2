
<script setup>
const projects = [
  {
    title: "Zona Coding",
    desc: "Website pembelajaran modern dengan tampilan yang menarik dan fitur interaktif.",
    image: "public/images/project1.webp",
    tech: [
      { name: "Vue JS", class: "bg-green-300" },
      { name: "Tailwind", class: "bg-yellow-300" },
    ],
  },
  {
    title: "Perpustakaan Digital",
    desc: "Website perpustakaan digital dengan fitur pencarian buku, dan baca buku digital.",
    image: "public/images/project2.webp",
    tech: [
      { name: "Laravel", class: "bg-blue-300" },
      { name: "MySQL", class: "bg-pink-300" },
    ],
  },
  {
    title: "Manajemen Toko",
    desc: "Website manajemen toko online dengan fitur CRUD, authentication, dan dashboard admin.",
    image: "public/images/project3.webp",
    tech: [
      { name: "Laravel", class: "bg-blue-300" },
      { name: "MySQL", class: "bg-pink-300" },
    ],
  },
];
</script>
<template>
  <section id="projects" class="relative min-h-screen px-6 md:px-16 py-[130px]">
    <!-- TITLE -->
    <img
      src="/public/images/pattern3.webp"
      alt=""
      class="absolute top-30 right-5 md:right-16 w-28 md:w-40 float opacity-60 pointer-events-none"
    />

    <div class="max-w-7xl mx-auto mb-14">
      <p
        class="inline-block bg-orange-500 text-white px-4 py-2 font-black rounded-2xl mb-5"
      >
        MY PROJECTS
      </p>

      <h1 class="text-4xl md:text-6xl font-black leading-tight mb-4">
        Selected Projects
      </h1>

      <p class="font-bold text-gray-700 text-lg max-w-2xl">
        Beberapa project yang pernah saya buat menggunakan Vue JS, Laravel, dan
        Tailwind CSS dengan desain modern dan responsive.
      </p>
    </div>

    <!-- PROJECT LIST -->
    <div class="max-w-7xl mx-auto grid md:grid-cols-2 lg:grid-cols-3 gap-10">
      <div
        v-for="(project, index) in projects"
        :key="index"
        class="bg-gray-50 border-4 border-gray-800 rounded-3xl overflow-hidden shadow-[10px_10px_0px_black] hover:-translate-y-2 transition duration-300"
      >
        <!-- IMAGE -->
        <img
          :src="project.image"
          alt="project"
          class="w-full h-[220px] object-cover border-b-4 border-gray-800"
        />

        <!-- CONTENT -->
        <div class="p-6">
          <div class="flex flex-wrap gap-3 mb-5">
            <span
              v-for="(tech, i) in project.tech"
              :key="i"
              :class="tech.class"
              class="border-2 border-gray-800 px-3 py-1 font-black text-sm"
            >
              {{ tech.name }}
            </span>
          </div>

          <h2 class="text-2xl font-black mb-3">{{ project.title }}</h2>

          <p class="font-bold text-gray-700 mb-6">
            {{ project.desc }}
          </p>
        </div>
      </div>
    </div>
  </section>
</template>