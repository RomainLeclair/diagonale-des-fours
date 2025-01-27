<template>
  <nav class="bg-white/90 backdrop-blur-sm shadow-lg fixed w-full z-10 top-0">
    <div class="container mx-auto px-6 py-4">
      <div class="flex justify-between items-center">
        <!-- Logo -->
        <div class="text-xl sm:text-2xl font-extrabold text-green-700">
          Diagonale Des Fours
        </div>

        <!-- Mobile menu button -->
        <div class="md:hidden">
          <button @click="isOpen = !isOpen" class="text-gray-500 hover:text-gray-600">
            <svg class="h-6 w-6" v-if="!isOpen" fill="none" viewBox="0 0 24 24" stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"/>
            </svg>
            <svg class="h-6 w-6" v-else fill="none" viewBox="0 0 24 24" stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"/>
            </svg>
          </button>
        </div>

        <!-- Desktop Navigation -->
        <div class="hidden md:flex items-center space-x-8">
          <router-link 
            v-for="link in links" 
            :key="link.path" 
            :to="link.path"
            class="text-gray-600 hover:text-green-600 transition duration-300"
          >
            {{ link.name }}
          </router-link>
          
          <a 
            href="https://www.klikego.com/inscription/diagonale-des-fours-2025/running-course-a-pied/1704922291482-2" 
            target="_blank"
            class="bg-gradient-to-r from-green-600 to-green-800 text-white font-semibold px-5 py-2 rounded-full shadow-lg hover:shadow-xl transition duration-300 transform hover:scale-105"
          >
            S'inscrire
          </a>
        </div>
      </div>

      <!-- Mobile Navigation -->
      <div 
        class="md:hidden transition-all duration-300"
        v-show="isOpen"
      >
        <div class="pt-4 pb-3 space-y-3">
          <router-link 
            v-for="link in links" 
            :key="link.path" 
            :to="link.path"
            @click="isOpen = false"
            class="block text-gray-600 hover:text-green-600 py-2 transition duration-300"
          >
            {{ link.name }}
          </router-link>
          
          <a 
            href="https://www.klikego.com/inscription/diagonale-des-fours-2025/running-course-a-pied/1704922291482-2" 
            target="_blank"
            class="block w-full text-center bg-gradient-to-r from-green-600 to-green-800 text-white font-semibold px-5 py-2 rounded-full shadow-lg hover:shadow-xl transition duration-300"
          >
            S'inscrire
          </a>
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'NavbarComponent',
  data() {
    return {
      isOpen: false,
      links: [
        { name: 'Accueil', path: '/' },
        { name: 'À propos', path: '/about' },
        { name: 'Événements', path: '/events' },
        { name: 'Contact', path: '/contact' },
        { name: 'Programme', path: '/programm' }
      ]
    }
  }
}
</script>