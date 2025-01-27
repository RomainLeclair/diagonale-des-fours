<template>
  <div class="min-h-screen">
    <!-- Hero Section -->
    <section class="relative h-[50vh] flex items-center justify-center bg-cover bg-center"
      :style="{ backgroundImage: `url(${require('@/assets/home_image.png')})` }">
      <div class="absolute inset-0 bg-gradient-to-b from-black/60 to-green-900/40"></div>
      <div class="relative z-10 text-center text-white p-4">
        <h1 class="text-5xl md:text-6xl font-black tracking-tight mb-4">
          Nos Parcours
        </h1>
        <p class="text-xl md:text-2xl font-light max-w-2xl mx-auto text-white/90">
          Choisissez votre défi parmi nos trois distances
        </p>
      </div>
    </section>

    <!-- Courses Section -->
    <section class="py-20 bg-gradient-to-b from-gray-50 to-white">
      <div class="container mx-auto px-6 max-w-7xl">
        <div class="grid grid-cols-1 md:grid-cols-3 gap-12">
          <!-- Trail 6km -->
          <div class="group relative">
            <div class="absolute inset-0 bg-gradient-to-r from-green-600/20 to-green-800/20 rounded-3xl transform rotate-2 transition-transform group-hover:rotate-3"></div>
            <div class="relative bg-white p-8 rounded-3xl shadow-xl transform transition-all duration-500 hover:scale-105">
              <div class="flex items-end mb-6">
                <span class="text-5xl font-bold text-gray-900">6</span>
                <span class="text-2xl font-medium text-gray-600 ml-2 mb-1">km</span>
              </div>
              <h3 class="text-2xl font-bold text-gray-900 mb-4">Trail Découverte</h3>
              <div class="space-y-4 text-gray-600 mb-8">
                <div class="flex items-center">
                  <svg class="w-5 h-5 mr-2 text-green-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 7h8m0 0v8m0-8l-8 8-4-4-6 6"/>
                  </svg>
                  <span>70m D+</span>
                </div>
                <div class="flex items-center">
                  <svg class="w-5 h-5 mr-2 text-green-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z"/>
                  </svg>
                  <span>1h estimé</span>
                </div>
                <p class="text-sm leading-relaxed">
                  Parfait pour une première expérience en trail. Un parcours accessible qui vous fera découvrir les plus beaux sentiers de Guenrouët.
                </p>
              </div>
              <a href="https://www.klikego.com/inscription/diagonale-des-fours-2025/running-course-a-pied/1704922291482-2" 
                target="_blank"
                class="inline-block w-full text-center bg-gradient-to-r from-green-600 to-green-800 text-white font-medium px-6 py-3 rounded-full hover:shadow-lg transition-all duration-300">
                S'inscrire
              </a>
            </div>
          </div>

          <!-- Trail 13km -->
          <div class="group relative">
            <div class="absolute inset-0 bg-gradient-to-r from-green-600/20 to-green-800/20 rounded-3xl transform rotate-2 transition-transform group-hover:rotate-3"></div>
            <div class="relative bg-white p-8 rounded-3xl shadow-xl transform transition-all duration-500 hover:scale-105">
              <div class="flex items-end mb-6">
                <span class="text-5xl font-bold text-gray-900">13,5</span>
                <span class="text-2xl font-medium text-gray-600 ml-2 mb-1">km</span>
              </div>
              <h3 class="text-2xl font-bold text-gray-900 mb-4">Trail Intermédiaire</h3>
              <div class="space-y-4 text-gray-600 mb-8">
                <div class="flex items-center">
                  <svg class="w-5 h-5 mr-2 text-green-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 7h8m0 0v8m0-8l-8 8-4-4-6 6"/>
                  </svg>
                  <span>120m D+</span>
                </div>
                <div class="flex items-center">
                  <svg class="w-5 h-5 mr-2 text-green-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z"/>
                  </svg>
                  <span>1h45 estimé</span>
                </div>
                <p class="text-sm leading-relaxed">
                  Un parcours équilibré offrant un beau challenge technique.
                </p>
              </div>
              <a href="https://www.klikego.com/inscription/diagonale-des-fours-2025/running-course-a-pied/1704922291482-2" 
                target="_blank"
                class="inline-block w-full text-center bg-gradient-to-r from-green-600 to-green-800 text-white font-medium px-6 py-3 rounded-full hover:shadow-lg transition-all duration-300">
                S'inscrire
              </a>
            </div>
          </div>

          <!-- Trail 24km -->
          <div class="group relative">
            <div class="absolute inset-0 bg-gradient-to-r from-green-600/20 to-green-800/20 rounded-3xl transform rotate-2 transition-transform group-hover:rotate-3"></div>
            <div class="relative bg-white p-8 rounded-3xl shadow-xl transform transition-all duration-500 hover:scale-105">
              <div class="flex items-end mb-6">
                <span class="text-5xl font-bold text-gray-900">24</span>
                <span class="text-2xl font-medium text-gray-600 ml-2 mb-1">km</span>
              </div>
              <h3 class="text-2xl font-bold text-gray-900 mb-4">Trail Expert</h3>
              <div class="space-y-4 text-gray-600 mb-8">
                <div class="flex items-center">
                  <svg class="w-5 h-5 mr-2 text-green-800" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 7h8m0 0v8m0-8l-8 8-4-4-6 6"/>
                  </svg>
                  <span>300m D+</span>
                </div>
                <div class="flex items-center">
                  <svg class="w-5 h-5 mr-2 text-green-800" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z"/>
                  </svg>
                  <span>2h30 estimé</span>
                </div>
                <p class="text-sm leading-relaxed">
                  Le parcours les traileurs expérimentés.
                </p>
              </div>
              <a href="https://www.klikego.com/inscription/diagonale-des-fours-2025/running-course-a-pied/1704922291482-2" 
                target="_blank"
                class="inline-block w-full text-center bg-gradient-to-r from-green-600 to-green-800 text-white font-medium px-6 py-3 rounded-full hover:shadow-lg transition-all duration-300">
                S'inscrire
              </a>
            </div>
          </div>
        </div>

        <!-- Section Informations Complémentaires -->
        <div class="mt-20 text-center">
          <h2 class="text-3xl font-bold text-gray-900 mb-8">Informations Pratiques</h2>
          <div class="grid grid-cols-1 md:grid-cols-4 gap-8">
            <div class="p-6 bg-gradient-to-br from-green-50 to-white rounded-2xl shadow-sm">
              <svg class="w-8 h-8 text-green-700 mx-auto mb-4" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 7V3m8 4V3m-9 8h10M5 21h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v12a2 2 0 002 2z"/>
              </svg>
              <h3 class="font-semibold mb-2">Date</h3>
              <p class="text-gray-600">05 Avril 2025</p>
            </div>
            <div class="p-6 bg-gradient-to-br from-green-50 to-white rounded-2xl shadow-sm">
              <svg class="w-8 h-8 text-green-700 mx-auto mb-4" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z"/>
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"/>
              </svg>
              <h3 class="font-semibold mb-2">Départ</h3>
              <p class="text-gray-600">Stade de Guenrouët</p>
            </div>
            <div class="p-6 bg-gradient-to-br from-green-50 to-white rounded-2xl shadow-sm">
              <svg class="w-8 h-8 text-green-700 mx-auto mb-4" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 10h18M7 15h1m4 0h1m-7 4h12a3 3 0 003-3V8a3 3 0 00-3-3H6a3 3 0 00-3 3v8a3 3 0 003 3z"/>
              </svg>
              <h3 class="font-semibold mb-2">Tarifs</h3>
              <p class="text-gray-600">De 5 à 20 €</p>
            </div>
            <div class="p-6 bg-gradient-to-br from-green-50 to-white rounded-2xl shadow-sm">
              <svg class="w-8 h-8 text-green-700 mx-auto mb-4" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M16 7a4 4 0 11-8 0 4 4 0 018 0zM12 14a7 7 0 00-7 7h14a7 7 0 00-7-7z"/>
              </svg>
              <h3 class="font-semibold mb-2">Places</h3>
              <p class="text-gray-600">Limitées à 500</p>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: 'eventsPage'
}
</script>