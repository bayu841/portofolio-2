<template>
  <section id="projects" class="min-h-screen px-6 md:px-16 py-[130px]">
    <!-- TITLE -->
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
      <!-- PROJECT CARD -->
      <div
        class="bg-gray-50 border-4 border-gray-800 rounded-3xl overflow-hidden shadow-[10px_10px_0px_black] hover:-translate-y-2 transition duration-300"
      >
        <!-- IMAGE -->
        <img
          src="/public/images/project1.webp"
          alt="project"
          class="w-full h-[220px] object-cover border-b-4 border-gray-800"
        />

        <!-- CONTENT -->
        <div class="p-6">
          <div class="flex flex-wrap gap-3 mb-5">
            <span
              class="bg-green-300 border-2 border-gray-800 px-3 py-1 font-black text-sm"
            >
              Vue JS
            </span>

            <span
              class="bg-yellow-300 border-2 border-gray-800 px-3 py-1 font-black text-sm"
            >
              Tailwind
            </span>
          </div>

          <h2 class="text-2xl font-black mb-3">Portfolio Website</h2>

          <p class="font-bold text-gray-700 mb-6">
            Website portfolio modern dengan style Neo Brutalism dan responsive
            design.
          </p>

          <!-- BUTTON -->
          <div class="flex gap-4">
            <a
              href="#"
              class="bg-orange-500 text-white border-4 border-gray-800 px-5 py-2 font-black shadow-[4px_4px_0px_black] hover:translate-x-1 hover:translate-y-1 hover:shadow-none transition duration-200"
            >
              Demo
            </a>

            <a
              href="#"
              class="bg-white border-4 border-gray-800 px-5 py-2 font-black shadow-[4px_4px_0px_black] hover:translate-x-1 hover:translate-y-1 hover:shadow-none transition duration-200"
            >
              Github
            </a>
          </div>
        </div>
      </div>

      <!-- PROJECT CARD -->
      <div
        class="bg-gray-50 border-4 border-gray-800 rounded-3xl overflow-hidden shadow-[10px_10px_0px_black] hover:-translate-y-2 transition duration-300"
      >
        <img
          src="/public/images/project2.webp"
          alt="project"
          class="w-full h-[220px] object-cover border-b-4 border-gray-800"
        />

        <div class="p-6">
          <div class="flex flex-wrap gap-3 mb-5">
            <span
              class="bg-blue-300 border-2 border-gray-800 px-3 py-1 font-black text-sm"
            >
              Laravel
            </span>

            <span
              class="bg-pink-300 border-2 border-gray-800 px-3 py-1 font-black text-sm"
            >
              MySQL
            </span>
          </div>

          <h2 class="text-2xl font-black mb-3">Book Store App</h2>

          <p class="font-bold text-gray-700 mb-6">
            Aplikasi toko buku online dengan fitur CRUD, authentication, dan
            dashboard admin.
          </p>

          <div class="flex gap-4">
            <a
              href="#"
              class="bg-orange-500 text-white border-4 border-gray-800 px-5 py-2 font-black shadow-[4px_4px_0px_black] hover:translate-x-1 hover:translate-y-1 hover:shadow-none transition duration-200"
            >
              Demo
            </a>

            <a
              href="#"
              class="bg-white border-4 border-gray-800 px-5 py-2 font-black shadow-[4px_4px_0px_black] hover:translate-x-1 hover:translate-y-1 hover:shadow-none transition duration-200"
            >
              Github
            </a>
          </div>
        </div>
      </div>

      <!-- PROJECT CARD -->
      <div
        class="bg-gray-50 border-4 border-gray-800 rounded-3xl overflow-hidden shadow-[10px_10px_0px_black] hover:-translate-y-2 transition duration-300"
      >
        <img
          src="/public/images/project3.webp"
          alt="project"
          class="w-full h-[220px] object-cover border-b-4 border-gray-800"
        />

        <div class="p-6">
          <div class="flex flex-wrap gap-3 mb-5">
            <span
              class="bg-orange-300 border-2 border-gray-800 px-3 py-1 font-black text-sm"
            >
              Vue JS
            </span>

            <span
              class="bg-green-300 border-2 border-gray-800 px-3 py-1 font-black text-sm"
            >
              Firebase
            </span>
          </div>

          <h2 class="text-2xl font-black mb-3">Task Management</h2>

          <p class="font-bold text-gray-700 mb-6">
            Website task management modern dengan realtime database dan
            responsive UI.
          </p>

          <div class="flex gap-4">
            <a
              href="#"
              class="bg-orange-500 text-white border-4 border-gray-800 px-5 py-2 font-black shadow-[4px_4px_0px_black] hover:translate-x-1 hover:translate-y-1 hover:shadow-none transition duration-200"
            >
              Demo
            </a>

            <a
              href="#"
              class="bg-white border-4 border-gray-800 px-5 py-2 font-black shadow-[4px_4px_0px_black] hover:translate-x-1 hover:translate-y-1 hover:shadow-none transition duration-200"
            >
              Github
            </a>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
