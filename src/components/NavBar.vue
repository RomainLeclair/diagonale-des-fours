<template>
    <nav class="bg-white shadow-lg fixed w-full z-10 top-0">
      <div class="container mx-auto px-6 py-4 flex justify-between items-center">
        <!-- Logo -->
        <div class="text-2xl font-extrabold text-blue-700">
          Diagonale Des Fours
        </div>
  
        <!-- Navigation Links -->
        <div class="space-x-8 hidden md:flex">
          <router-link to="/" class="text-gray-600 hover:text-blue-600 transition duration-300 ease-in-out">Accueil</router-link>
          <router-link to="/about" class="text-gray-600 hover:text-blue-600 transition duration-300 ease-in-out">À propos</router-link>
          <router-link to="/events" class="text-gray-600 hover:text-blue-600 transition duration-300 ease-in-out">Événements</router-link>
          <router-link to="/contact" class="text-gray-600 hover:text-blue-600 transition duration-300 ease-in-out">Contact</router-link>
          <router-link to="/programm" class="text-gray-600 hover:text-blue-600 transition duration-300 ease-in-out">Programme</router-link>
        </div>
  
        <!-- Signup Button -->
        <div>
          <router-link to="/signup" class="bg-blue-600 text-white font-semibold px-5 py-2 rounded-full shadow-lg hover:bg-blue-700 transition duration-300 ease-in-out">
            S'inscrire
          </router-link>
        </div>
      </div>
    </nav>
  </template>
  
  <script>
  export default {
    name: 'NavbarComponent'
  }
  </script>
  