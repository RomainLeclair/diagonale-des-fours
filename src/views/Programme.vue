<template>
    <div class="min-h-screen bg-gradient-to-b from-gray-900 to-gray-800">
      <!-- Hero Section avec effet parallax -->
      <section class="relative h-[50vh] flex items-center justify-center bg-cover bg-center bg-fixed"
        :style="{ backgroundImage: `url(${require('@/assets/home_image.png')})` }">
        <div class="absolute inset-0 bg-gradient-to-b from-black/70 via-transparent to-gray-900"></div>
        <div class="relative z-10 text-center text-white p-4">
          <h1 class="text-5xl md:text-7xl font-black tracking-tight mb-4 animate-fade-in-down">
            Programme
          </h1>
          <p class="text-xl md:text-2xl font-light max-w-2xl mx-auto text-white/90 animate-fade-in-up">
            Une journée exceptionnelle vous attend
          </p>
        </div>
      </section>

      <!-- Nouvelle section Programme -->
        <section class="relative py-20">
          <div class="container mx-auto px-6 max-w-5xl">
            <ProgramTable />
          </div>
        </section>
  
      <!-- Programme Section avec effet de profondeur -->
      <section class="relative py-20">
        <!-- Effet de background avec formes géométriques -->
        <div class="absolute inset-0 overflow-hidden">
          <div class="absolute top-0 left-0 w-96 h-96 bg-blue-500/10 rounded-full filter blur-3xl"></div>
          <div class="absolute bottom-0 right-0 w-96 h-96 bg-purple-500/10 rounded-full filter blur-3xl"></div>
        </div>
  
        <div class="container mx-auto px-6 max-w-5xl relative z-10">
          <!-- Timeline verticale avec effet de gradient -->
          <div class="relative">
            <!-- Ligne verticale avec gradient -->
            <div class="absolute left-0 md:left-1/2 transform md:-translate-x-1/2 top-0 bottom-0 w-1 bg-gradient-to-b from-blue-500 via-purple-500 to-pink-500"></div>
  
            <!-- Vendredi -->
            <div class="mb-20 relative">
              <div class="flex items-center justify-center md:justify-start mb-12">
                <div class="bg-gradient-to-r from-blue-600 to-blue-400 p-4 rounded-2xl shadow-xl transform hover:scale-105 transition-all duration-300">
                  <h2 class="text-3xl font-bold text-white">Vendredi 14 Juillet</h2>
                </div>
              </div>
  
              <div class="space-y-12">
                <TimelineItem 
                  time="14h - 19h"
                  title="Retrait des dossards"
                  location="Centre ville de Chambéry"
                  bgImage="url('/home_image.png')"
                  side="right"
                />
                <TimelineItem 
                  time="18h00"
                  title="Briefing d'avant course"
                  location="Salle des fêtes"
                  bgImage="url('/home_image.png')"
                  side="left"
                />
              </div>
            </div>
  
            <!-- Samedi -->
            <div class="relative">
              <div class="flex items-center justify-center md:justify-end mb-12">
                <div class="bg-gradient-to-r from-purple-600 to-pink-500 p-4 rounded-2xl shadow-xl transform hover:scale-105 transition-all duration-300">
                  <h2 class="text-3xl font-bold text-white">Samedi 15 Juillet - Jour J</h2>
                </div>
              </div>
  
              <div class="space-y-12">
                <TimelineItem 
                  time="5h00"
                  title="Départ du 24km"
                  location="Place de l'Hôtel de Ville"
                  bgImage="url('/home_image.png')"
                  side="left"
                  color="purple"
                />
                <TimelineItem 
                  time="7h00"
                  title="Départ du 13km"
                  location="Place de l'Hôtel de Ville"
                  bgImage="url('/home_image.png')"
                  side="right"
                  color="indigo"
                />
                <TimelineItem 
                  time="8h30"
                  title="Départ du 6km"
                  location="Place de l'Hôtel de Ville"
                  bgImage="url('/home_image.png')"
                  side="left"
                  color="blue"
                />
              </div>
            </div>
          </div>
  

  

  
          <!-- Message important avec effet de verre -->
          <div class="mt-12 relative overflow-hidden">
            <div class="absolute inset-0 bg-gradient-to-r from-yellow-500/20 to-orange-500/20 backdrop-blur-xl"></div>
            <div class="relative backdrop-blur-lg rounded-3xl p-8 border border-yellow-400/30">
              <h3 class="text-2xl font-bold text-white mb-4">Informations importantes</h3>
              <ul class="space-y-4 text-white/90">
                <li class="flex items-center space-x-3">
                  <svg class="w-6 h-6 text-yellow-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 9v2m0 4h.01m-6.938 4h13.856c1.54 0 2.502-1.667 1.732-3L13.732 4c-.77-1.333-2.694-1.333-3.464 0L3.34 16c-.77 1.333.192 3 1.732 3z"/>
                  </svg>
                  <span>Certificat médical obligatoire de moins d'un an</span>
                </li>
                <li class="flex items-center space-x-3">
                  <svg class="w-6 h-6 text-yellow-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 9v2m0 4h.01m-6.938 4h13.856c1.54 0 2.502-1.667 1.732-3L13.732 4c-.77-1.333-2.694-1.333-3.464 0L3.34 16c-.77 1.333.192 3 1.732 3z"/>
                  </svg>
                  <span>Matériel obligatoire à vérifier avant le départ</span>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </section>
    </div>
  </template>
  
  <script>
  const TimelineItem = {
    props: {
      time: String,
      title: String,
      location: String,
      bgImage: String,
      side: String,
      color: {
        type: String,
        default: 'blue'
      }
    },
    template: `
      <div :class="['relative flex items-center', side === 'left' ? 'md:flex-row-reverse' : '']">
        <div class="w-full md:w-1/2 p-4">
          <div class="bg-gradient-to-br" :class="[
            color === 'purple' ? 'from-purple-600/90 to-purple-800/90' : 
            color === 'indigo' ? 'from-indigo-600/90 to-indigo-800/90' : 
            'from-blue-600/90 to-blue-800/90'
          ]" class="rounded-2xl p-6 transform hover:scale-105 transition-all duration-300 backdrop-blur-lg border border-white/10">
            <div class="text-3xl font-bold text-white mb-2">{{ time }}</div>
            <h3 class="text-xl font-semibold text-white">{{ title }}</h3>
            <p class="text-white/80 mt-2">{{ location }}</p>
          </div>
        </div>
        <div class="absolute left-0 md:left-1/2 transform md:-translate-x-1/2 w-4 h-4 rounded-full bg-white shadow-lg"></div>
      </div>
    `
  };
  
  import ProgramTable from '@/components/ProgramTable.vue'
  export default {
    name: 'ProgrammePage',
    components: {
      TimelineItem,
      ProgramTable
    }
  }
  </script>
  
  <style scoped>
  @keyframes fade-in-down {
    0% {
      opacity: 0;
      transform: translateY(-20px);
    }
    100% {
      opacity: 1;
      transform: translateY(0);
    }
  }
  
  @keyframes fade-in-up {
    0% {
      opacity: 0;
      transform: translateY(20px);
    }
    100% {
      opacity: 1;
      transform: translateY(0);
    }
  }
  
  .animate-fade-in-down {
    animation: fade-in-down 1s ease-out;
  }
  
  .animate-fade-in-up {
    animation: fade-in-up 1s ease-out;
  }
  </style>