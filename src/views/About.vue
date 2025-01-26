<template>
  <div class="pt-24 bg-gradient-to-b from-green-50 to-white min-h-screen">
    <div class="container mx-auto px-4 sm:px-6 max-w-4xl">
      <div class="text-center mb-16">
        <h1 class="text-4xl md:text-5xl font-bold text-gray-900 mb-4">
          À propos de 
          <span class="text-transparent bg-clip-text bg-gradient-to-r from-green-600 to-green-800">
            La Diagonale des Fours
          </span>
        </h1>
        <p class="text-xl text-gray-600">Une course nature au cœur de Guenrouët</p>
      </div>

      <div class="prose prose-lg mx-auto space-y-6 text-gray-600">
        <div class="bg-white rounded-2xl shadow-xl p-8 mb-8 border-l-4 border-green-600">
          <p class="mb-6">
            Notre petite aventure commence en août 2021 et est célébrée un certain 3 avril 2022 avenue Foch à Paris !
          </p>
          
          <p class="mb-6">
            De ce groupe nait l'idée d'un rassemblement pour réunir tous les coureurs et randonneurs, et autres sportifs de tous horizons, lors d'une sortie « unique ».
          </p>

          <div class="bg-green-50 p-6 my-8 rounded-xl">
            <p class="font-medium text-green-900">
              « La Diagonale des Fours » voit le jour le 1er avril 2023, du Clandre vers Peslan avec 4 distances, 24, 13, 6 et 3 km pour les enfants. Nous sommes 107 pour le « Test ».
            </p>
          </div>

          <p class="mb-6">
            Par l'association « Athlétic Run'Isac », nous souhaitons officialiser et pérenniser ce rassemblement, voire d'autres.
          </p>

          <p class="mb-6">
            « Athlétic Run'Isac » a pour objectif de promouvoir la course à pied et la randonnée, avant tout en loisir, sur notre belle commune.
          </p>

          <p class="mb-6">
            Notre dénomination, comme une évidence, rend hommage à nos ainés qui, de 1967 à 1985, ont porté haut les couleurs de Guenrouët sous l'égide de « L'Athlétic Club de l'Isac ».
          </p>

          <div class="bg-green-50 p-6 my-8 rounded-xl">
            <p class="font-medium text-green-900">
              Nous n'avons pas vocation à être « club ». Nous souhaitons juste, en toute simplicité, créer une dynamique autour de la course à pied et la randonnée.
            </p>
          </div>

          <p class="mb-8">
            Nous souhaitons saluer tous les coureurs et randonneurs et les invitons à nous rejoindre le samedi 6 avril après-midi pour la 2ème édition de « La Diagonale des fours » !
          </p>

          <p class="text-center font-semibold text-xl text-green-700 mt-8">
            Sportivement, évidemment…
          </p>
        </div>

        <!-- Info Card -->
        <div class="grid grid-cols-1 md:grid-cols-3 gap-6 mt-12">
          <div class="bg-white p-6 rounded-xl shadow-lg border-t-4 border-green-600">
            <h3 class="font-bold text-xl mb-2 text-green-800">Distances</h3>
            <p>6km, 12km et 24km</p>
            <p class="text-sm text-gray-500">+ Course enfants gratuite</p>
          </div>
          <div class="bg-white p-6 rounded-xl shadow-lg border-t-4 border-green-600">
            <h3 class="font-bold text-xl mb-2 text-green-800">Lieu</h3>
            <p>Stade Municipal</p>
            <p class="text-sm text-gray-500">Guenrouët (44)</p>
          </div>
          <div class="bg-white p-6 rounded-xl shadow-lg border-t-4 border-green-600">
            <h3 class="font-bold text-xl mb-2 text-green-800">Services</h3>
            <p>Bar et restauration</p>
            <p class="text-sm text-gray-500">Douches et vestiaires</p>
          </div>
        </div>

        <!-- Call to action -->
        <div class="text-center mt-12">
          <a 
            href="https://www.klikego.com/inscription/diagonale-des-fours-2025/running-course-a-pied/1704922291482-2"
            target="_blank"
            class="inline-block px-8 py-4 bg-gradient-to-r from-green-600 to-green-800 text-white font-medium rounded-full hover:shadow-lg transform transition-all duration-300 hover:scale-105"
          >
            S'inscrire à la course
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'AboutPage'
}
</script>