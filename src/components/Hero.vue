<template>
  <section class="bg-gradient-to-r from-orange-600 to-orange-400 text-white py-20">
    <div class="max-w-7xl mx-auto px-6 flex flex-col md:flex-row items-center gap-10">
      <!-- Texto -->
      <div class="flex-1 text-center md:text-left">
        <h1 class="text-4xl md:text-5xl font-extrabold leading-tight">
          Dales una <span class="text-orange-100 float inline-block">segunda</span><br />
          oportunidad
        </h1>
        <p class="mt-6 text-lg text-orange-100">
          Cada perrito merece un hogar lleno de amor. En <strong>Huellas Vivas</strong> conectamos
          corazones que buscan dar y recibir amor incondicional.
        </p>
        <div class="mt-8 flex flex-col md:flex-row justify-center md:justify-start gap-4">
            <a
                href="#perritos"
                class="bg-white text-orange-600 font-semibold px-6 py-2 rounded shadow hover:bg-orange-100 transition w-full md:w-auto text-center"
            >
                Conoce a nuestros perritos
            </a>
            <a
                href="#adopcion"
                class="bg-white/80 text-orange-700 font-semibold px-6 py-2 rounded shadow hover:bg-white transition w-full md:w-auto text-center"
            >
                Cómo adoptar
            </a>
        </div>
      </div>

      <!-- Imagen -->
      <div class="flex-1 relative">
        <img
          src="/img/perro.jpg"
          alt="Perrito adorable"
          class="w-full rounded-xl shadow-lg object-cover float"
        />
        <div
          class="absolute bottom-2 right-2 bg-orange-100 text-orange-800 text-sm font-semibold px-4 py-1 rounded-full shadow"
        >
          ¡Disponible para adopción!
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
// No logic yet
</script>
