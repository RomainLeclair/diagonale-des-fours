<template>
    <div class="space-y-4">
      <div v-for="(event, index) in events" :key="index"
        class="bg-gradient-to-r from-gray-800/50 to-gray-800/30 backdrop-blur-sm rounded-2xl p-6 border border-gray-700/50 hover:border-blue-500/50 transition-all duration-300 group">
        <div class="flex items-center space-x-8">
          <div class="w-24">
            <span class="text-2xl font-bold bg-gradient-to-r from-blue-400 to-purple-400 text-transparent bg-clip-text">
              {{ event.time }}
            </span>
          </div>
          <div class="flex-1">
            <h3 class="text-xl font-semibold text-white group-hover:text-blue-400 transition-colors duration-300">
              {{ event.event }}
            </h3>
            <p class="text-gray-400 mt-1">
              {{ event.description }}
            </p>
          </div>
          <div class="w-8 opacity-0 group-hover:opacity-100 transition-opacity duration-300">
            <svg class="w-6 h-6 text-blue-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path strokeLinecap="round" strokeLinejoin="round" strokeWidth={2} d="M9 5l7 7-7 7"/>
            </svg>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'ProgramTable',
    data() {
      return {
        events: [
          {
            time: "12:00",
            event: "Ouverture du Village",
            description: "Restauration et buvette (CB acceptée)"
          },
          {
            time: "14:00",
            event: "Départ Trail 24 km",
            description: "Point de départ : Stade de Guenrouët"
          },
          {
            time: "14:30",
            event: "Départ Trail 13 km",
            description: "Point de départ : Stade de Guenrouët"
          },
          {
            time: "15:00",
            event: "Départ Trail 6 km",
            description: "Point de départ : Stade de Guenrouët"
          },
          
          {
            time: "16:00",
            event: "Départ Course 600m",
            description: "Course enfants (6-8 ans)"
          },
          {
            time: "16:30",
            event: "Départ Course 1000m",
            description: "Course enfants (9-11 ans)"
          },
          
          {
            time: "17:00",
            event: "Remise des prix",
            description: "Podiums toutes catégories"
          },
          {
            time: "18:00",
            event: "Concert de clôture",
            description: "Animation musicale gratuite"
          }
        ]
      }
    }
  }
  </script>