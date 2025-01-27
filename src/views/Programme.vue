<template>
  <div class="min-h-screen bg-gradient-to-b from-gray-900 to-gray-800">
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

    <section class="relative py-20">
      <div class="container mx-auto px-6 max-w-5xl">
        <ProgramTable />
      </div>
    </section>

    <!-- Section Informations -->
    <section class="relative pb-20">
      <div class="container mx-auto px-6 max-w-5xl relative z-10">
        <div class="relative overflow-hidden">
          <div class="relative backdrop-blur-lg rounded-3xl p-8 bg-white/5 border border-white/10">
            <h3 class="text-2xl font-bold text-white mb-4">Informations importantes</h3>
            <ul class="space-y-4 text-white/90">
              <li class="flex items-center space-x-3">
                <svg class="w-6 h-6 text-green-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 9v2m0 4h.01m-6.938 4h13.856c1.54 0 2.502-1.667 1.732-3L13.732 4c-.77-1.333-2.694-1.333-3.464 0L3.34 16c-.77 1.333.192 3 1.732 3z"/>
                </svg>
                <span>Parcours compliqués</span>
              </li>
              <li class="flex items-center space-x-3">
              </li>
            </ul>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import ProgramTable from '@/components/ProgramTable.vue'
export default {
  name: 'ProgrammePage',
  components: {
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