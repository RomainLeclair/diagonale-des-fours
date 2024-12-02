<template>
  <div class="min-h-screen">
    <!-- Hero Section plus compact -->
    <section class="relative h-[40vh] flex items-center justify-center bg-cover bg-center"
      :style="{ backgroundImage: `url(${require('@/assets/home_image.png')})` }">
      <div class="absolute inset-0 bg-gradient-to-b from-black/60 to-black/40"></div>
      <div class="relative z-10 text-center text-white p-4">
        <h1 class="text-5xl md:text-6xl font-black tracking-tight mb-4">
          Contactez-nous
        </h1>
        <p class="text-xl md:text-2xl font-light max-w-2xl mx-auto text-white/90">
          Notre équipe est à votre écoute
        </p>
      </div>
    </section>

    <!-- Contact Section -->
    <section class="py-20 bg-gradient-to-b from-gray-50 to-white">
      <div class="container mx-auto px-6 max-w-7xl">
        <div class="grid grid-cols-1 md:grid-cols-2 gap-16">
          <!-- Informations de contact -->
          <div class="space-y-12">
            <div>
              <h2 class="text-3xl font-bold text-gray-900 mb-8">
                Nos coordonnées
              </h2>
              <div class="space-y-8">
                <!-- Adresse -->
                <div class="group">
                  <div class="flex items-start space-x-4">
                    <div class="p-3 bg-blue-50 rounded-xl group-hover:bg-blue-100 transition-colors duration-300">
                      <svg class="w-6 h-6 text-blue-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" 
                          d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z"/>
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" 
                          d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"/>
                      </svg>
                    </div>
                    <div>
                      <h3 class="text-lg font-semibold text-gray-900 mb-1">Adresse</h3>
                      <p class="text-gray-600 leading-relaxed">
                        Guenrouët<br>
                        44530 Guenrouët<br>
                        France
                      </p>
                    </div>
                  </div>
                </div>

                <!-- Téléphone -->
                <div class="group">
                  <div class="flex items-start space-x-4">
                    <div class="p-3 bg-green-50 rounded-xl group-hover:bg-green-100 transition-colors duration-300">
                      <svg class="w-6 h-6 text-green-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" 
                          d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z"/>
                      </svg>
                    </div>
                    <div>
                      <h3 class="text-lg font-semibold text-gray-900 mb-1">Téléphone</h3>
                      <p class="text-gray-600">
                        <a href="tel:+33612345678" class="hover:text-green-600 transition-colors duration-300">
                          +33 6 xx xx xx
                        </a>
                      </p>
                    </div>
                  </div>
                </div>

                <!-- Email -->
                <div class="group">
                  <div class="flex items-start space-x-4">
                    <div class="p-3 bg-purple-50 rounded-xl group-hover:bg-purple-100 transition-colors duration-300">
                      <svg class="w-6 h-6 text-purple-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" 
                          d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"/>
                      </svg>
                    </div>
                    <div>
                      <h3 class="text-lg font-semibold text-gray-900 mb-1">Email</h3>
                      <p class="text-gray-600">
                        <a href="mailto:contact@diagonaledesfours.fr" class="hover:text-purple-600 transition-colors duration-300">
                          athelticrunisac@gmail.com
                        </a>
                      </p>
                    </div>
                  </div>
                </div>
              </div>
            </div>

            <!-- Réseaux sociaux -->
            <div>
              <h3 class="text-lg font-semibold text-gray-900 mb-4">Suivez-nous</h3>
              <div class="flex space-x-4">
                <a href="#" class="p-3 bg-gray-50 rounded-full hover:bg-gray-100 transition-colors duration-300">
                  <svg class="w-5 h-5 text-gray-700" fill="currentColor" viewBox="0 0 24 24">
                    <path d="M24 12.073c0-6.627-5.373-12-12-12s-12 5.373-12 12c0 5.99 4.388 10.954 10.125 11.854v-8.385H7.078v-3.47h3.047V9.43c0-3.007 1.792-4.669 4.533-4.669 1.312 0 2.686.235 2.686.235v2.953H15.83c-1.491 0-1.956.925-1.956 1.874v2.25h3.328l-.532 3.47h-2.796v8.385C19.612 23.027 24 18.062 24 12.073z"/>
                  </svg>
                </a>
                <a href="#" class="p-3 bg-gray-50 rounded-full hover:bg-gray-100 transition-colors duration-300">
                  <svg class="w-5 h-5 text-gray-700" fill="currentColor" viewBox="0 0 24 24">
                    <path d="M12 0C8.74 0 8.333.015 7.053.072 5.775.132 4.905.333 4.14.63c-.789.306-1.459.717-2.126 1.384S.935 3.35.63 4.14C.333 4.905.131 5.775.072 7.053.012 8.333 0 8.74 0 12s.015 3.667.072 4.947c.06 1.277.261 2.148.558 2.913.306.788.717 1.459 1.384 2.126.667.666 1.336 1.079 2.126 1.384.766.296 1.636.499 2.913.558C8.333 23.988 8.74 24 12 24s3.667-.015 4.947-.072c1.277-.06 2.148-.262 2.913-.558.788-.306 1.459-.718 2.126-1.384.666-.667 1.079-1.335 1.384-2.126.296-.765.499-1.636.558-2.913.06-1.28.072-1.687.072-4.947s-.015-3.667-.072-4.947c-.06-1.277-.262-2.149-.558-2.913-.306-.789-.718-1.459-1.384-2.126C21.319 1.347 20.651.935 19.86.63c-.765-.297-1.636-.499-2.913-.558C15.667.012 15.26 0 12 0zm0 2.16c3.203 0 3.585.016 4.85.071 1.17.055 1.805.249 2.227.415.562.217.96.477 1.382.896.419.42.679.819.896 1.381.164.422.36 1.057.413 2.227.057 1.266.07 1.646.07 4.85s-.015 3.585-.074 4.85c-.061 1.17-.256 1.805-.421 2.227-.224.562-.479.96-.899 1.382-.419.419-.824.679-1.38.896-.42.164-1.065.36-2.235.413-1.274.057-1.649.07-4.859.07-3.211 0-3.586-.015-4.859-.074-1.171-.061-1.816-.256-2.236-.421-.569-.224-.96-.479-1.379-.899-.421-.419-.69-.824-.9-1.38-.165-.42-.359-1.065-.42-2.235-.045-1.26-.061-1.649-.061-4.844 0-3.196.016-3.586.061-4.861.061-1.17.255-1.814.42-2.234.21-.57.479-.96.9-1.381.419-.419.81-.689 1.379-.898.42-.166 1.051-.361 2.221-.421 1.275-.045 1.65-.06 4.859-.06l.045.03zm0 3.678c-3.405 0-6.162 2.76-6.162 6.162 0 3.405 2.76 6.162 6.162 6.162 3.405 0 6.162-2.76 6.162-6.162 0-3.405-2.76-6.162-6.162-6.162zM12 16c-2.21 0-4-1.79-4-4s1.79-4 4-4 4 1.79 4 4-1.79 4-4 4zm7.846-10.405c0 .795-.646 1.44-1.44 1.44-.795 0-1.44-.646-1.44-1.44 0-.794.646-1.439 1.44-1.439.793-.001 1.44.645 1.44 1.439z"/>
                  </svg>
                </a>
              </div>
            </div>
          </div>

          <!-- Carte -->
          <div class="relative h-[500px] rounded-3xl overflow-hidden shadow-xl">
            <iframe 
            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d21434.037890075275!2d-1.9340385!3d47.5276584!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x480f8c89b0f6d0d9%3A0x40d37521e0d73b0!2s44530%20Guenrou%C3%ABt!5e0!3m2!1sfr!2sfr!4v1701515632024!5m2!1sfr!2sfr" 
              width="100%" 
              height="100%" 
              style="border:0;" 
              allowfullscreen="" 
              loading="lazy"
              class="filter grayscale"
            ></iframe>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: 'ContactPage'
}
</script>

<style scoped>
.gradient-text {
  background-clip: text;
  -webkit-background-clip: text;
  color: transparent;
}
</style>
  