<template>
  <div class="overflow-hidden">
    <!-- Hero Section avec effet parallaxe -->
    <section 
      class="relative min-h-screen flex items-center justify-center bg-cover bg-fixed bg-center transition-all duration-700"
      :style="{ backgroundImage: `url(${require('@/assets/home_image.png')})` }"
      v-parallax="0.5"
    >
      <div class="absolute inset-0 bg-gradient-to-b from-black/40 via-black/20 to-black/60"></div>

      <div class="relative z-10 text-center text-white p-4 max-w-5xl mx-auto transform transition-all duration-700 translate-y-0 hover:translate-y-[-10px]">
        <h1 class="text-6xl md:text-8xl font-black tracking-tight leading-none mb-6 bg-clip-text text-transparent bg-gradient-to-r from-white to-white/80">
          La Diagonale des Fours<br/>
        </h1>
        <p class="mt-8 text-xl md:text-2xl max-w-2xl mx-auto font-light leading-relaxed text-white/90">
          Une aventure unique à travers les paysages les plus spectaculaires de nos montagnes.
        </p>
        <div class="mt-12 space-x-6">
          <router-link 
            to="/signup" 
            class="inline-block bg-white text-black font-medium px-8 py-4 rounded-full hover:bg-white/90 transition-all duration-300 ease-out transform hover:scale-105 hover:shadow-2xl"
          >
            S'inscrire
          </router-link>
          <router-link 
            to="/events" 
            class="inline-block bg-transparent border border-white/30 backdrop-blur-sm text-white font-medium px-8 py-4 rounded-full hover:bg-white/10 transition-all duration-300 ease-out transform hover:scale-105"
          >
            Découvrir
          </router-link>
        </div>
      </div>

      <!-- Scroll indicator -->
      <div class="absolute bottom-10 left-1/2 transform -translate-x-1/2 animate-bounce">
        <svg class="w-6 h-6 text-white/70" fill="none" stroke="currentColor" viewBox="0 0 24 24">
          <path strokeLinecap="round" strokeLinejoin="round" strokeWidth="2" d="M19 14l-7 7m0 0l-7-7m7 7V3"/>
        </svg>
      </div>
    </section>

    <!-- Presentation Section avec design moderne -->
    <section class="py-24 bg-gradient-to-b from-gray-50 to-white">
      <div class="container mx-auto px-6 max-w-7xl">
        <div class="grid grid-cols-1 md:grid-cols-2 gap-16 items-center">
          <!-- Image avec effet moderne -->
          <div class="relative group">
            <div class="absolute inset-0 bg-gradient-to-r from-blue-600/20 to-purple-600/20 rounded-3xl transform rotate-3 transition-transform group-hover:rotate-6"></div>
            <img 
              :src="require('@/assets/home_image.png')" 
              alt="Trail running" 
              class="relative rounded-3xl shadow-2xl transform transition-all duration-500 group-hover:scale-105 object-cover w-full h-[600px]"
            >
          </div>

          <!-- Contenu avec typographie moderne -->
          <div class="space-y-8">
            <h2 class="text-4xl md:text-5xl font-bold text-gray-900 leading-tight">
              L'esprit de<br/>
              <span class="text-transparent bg-clip-text bg-gradient-to-r from-blue-600 to-purple-600">l'aventure</span>
            </h2>
            <p class="text-lg text-gray-600 leading-relaxed">
              Parcourez des sentiers uniques à travers des paysages à couper le souffle. Notre trail vous emmène au cœur d'une nature préservée, où chaque kilomètre raconte une histoire et chaque montée révèle un nouveau défi.
            </p>
            <div class="grid grid-cols-2 gap-8 pt-8">
              <div>
                <div class="text-3xl font-bold text-gray-900">42km</div>
                <div class="text-gray-500">Distance</div>
              </div>
              <div>
                <div class="text-3xl font-bold text-gray-900">2500m</div>
                <div class="text-gray-500">Dénivelé</div>
              </div>
            </div>
            <router-link 
              to="/events" 
              class="inline-block mt-8 px-8 py-4 bg-gradient-to-r from-blue-600 to-purple-600 text-white font-medium rounded-full hover:shadow-lg transform transition-all duration-300 hover:scale-105"
            >
              En savoir plus
            </router-link>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: 'HomePage',
  directives: {
    parallax: {
      mounted(el, binding) {
        window.addEventListener('scroll', () => {
          const speed = binding.value || 0.5
          const yPos = -(window.pageYOffset * speed)
          el.style.backgroundPositionY = `${yPos}px`
        })
      },
      // eslint-disable-next-line
      unmounted(el) { // eslint-disable-next-line
        window.removeEventListener('scroll', () => {})
      }
    }
  }
}
</script>

<style scoped>
@keyframes gradient {
  0% { background-position: 0% 50%; }
  50% { background-position: 100% 50%; }
  100% { background-position: 0% 50%; }
}

.bg-gradient-animate {
  background-size: 200% 200%;
  animation: gradient 15s ease infinite;
}
</style>