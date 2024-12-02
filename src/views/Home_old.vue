<template>
  <div>
    <!-- Hero Section -->
    <section class="relative h-screen flex items-center justify-center bg-cover bg-center" style="background-image: url('https://source.unsplash.com/1600x900/?trail,landscape');">
      <div class="absolute inset-0 bg-gradient-to-b from-black via-transparent to-black opacity-75"></div> <!-- Overlay avec un dégradé -->

      <!-- Texte principal -->
      <div class="relative z-10 text-center text-white p-4">
        <h1 class="text-5xl md:text-7xl font-extrabold tracking-tight leading-tight mb-4">
          Découvrez l'Aventure<br /> avec Tikentrail
        </h1>
        <p class="mt-4 text-lg md:text-2xl max-w-xl mx-auto font-light leading-relaxed">
          Participez à des parcours de trail dans des paysages à couper le souffle.
        </p>
        <div class="mt-8 space-x-4">
          <router-link to="/signup" class="inline-block bg-blue-600 text-white font-semibold px-6 py-3 rounded-full shadow-lg hover:bg-blue-700 transition duration-300 ease-in-out">
            Rejoignez-nous
          </router-link>
          <router-link to="/events" class="inline-block bg-transparent border border-white text-white font-semibold px-6 py-3 rounded-full hover:bg-white hover:text-blue-600 transition duration-300 ease-in-out">
            Voir les événements
          </router-link>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: 'HomePage'
}
</script>

