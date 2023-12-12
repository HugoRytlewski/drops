<template>
    <title>Drops</title>
    <nav class="flex items-center justify-between p-4 fixed top-0 left-0 right-0 bg-neutral-950 border-b border-gray-800 z-50">
      <img src="./assets/menu.svg" alt="Menu" class="h-6 w-6" />
      <h1 class="text-2xl text-white font-bold">DROPS</h1>
      <img src="./assets/panier.svg" alt="Cart" class="h-6 w-6 fill-white text-white" />
    </nav>

    <footer class="z-20 fixed inset-x-0 bottom-10 mx-auto bg-black w-56 h-14 rounded-full flex justify-around items-center">
      <img src="./assets/accueil.svg" alt="Home" class="hover:opacity-75 duration-200 h-6 w-6 text-white" />
      <img src="./assets/loupeb.svg" alt="Search" class="hover:opacity-75 duration-200 vh-6 w-6 text-white" />
      <img src="./assets/coeur.svg" alt="Favorite" class="hover:opacity-75 duration-200 h-6 w-6 text-white" />
      <img src="./assets/compte.svg" alt="Profile" class="hover:opacity-75 duration-200 h-6 w-6 text-white" />
    </footer>

    <div class="z-0 flex flex-col justify-center md:items-center min-h-screen bg-neutral-950 text-white">
      <div class="pt-16 pb-4 px-4">
        <div class="mt-4  md:mt-[-7rem] md:flex flex-col items-center justify-center ">

          <div class="bg-white text-black rounded-full flex items-center md:w-96 p-3">
            <img src="./assets/loupe.svg" alt="Search" class="h-5 w-5 " />
            <input class="ml-2 outline-none bg-transparent flex-grow" type="text" placeholder="Que cherchez vous?"/>
          </div>
          <div class="mt-3 bg-green-600 rounded-full flex items-center justify-left gap-2 p-3 md:w-96">
            <img src="./assets/pin.svg" alt="Arrow right" class="h-5 w-5" />
            <span>Limoges , France</span>
          </div>
        </div>
        <div class="flex overflow-x-auto snap-x snap-mandatory mt-10">
  <div class=" shrink-0 w-full flex flex-none gap-10">
    <!-- Premier élément du slider -->
    <div class="min-w-full md:min-w-0">
      <div class="bg-white text-black rounded-t-xl p-3">
        <span class="font-semibold">Tendances</span>
      </div>
      <div class="relative bg-white rounded-b-xl p-3 flex flex-col items-center">
        <img src="./assets/chaussure.png" alt="Featured Product" class="h-40 w-full object-cover rounded-t-lg" />
        <div class="absolute bottom-0 left-0 right-0 p-3 bg-black text-white hover:opacity-75 duration-200">
          <p>Vente de fin d'année jusqu'à 90 % - Achetez maintenant !</p>
        </div>
      </div>
    </div>
    <div class="min-w-full md:min-w-0">
      <div class="bg-white text-black rounded-t-xl p-3">
        <span class="font-semibold">Tendances</span>
      </div>
      <div class="relative bg-white rounded-b-xl p-3 flex flex-col items-center">
        <img src="./assets/chaussure.png" alt="Featured Product" class="h-40 w-full object-cover rounded-t-lg" />
        <div class="absolute bottom-0 left-0 right-0 p-3 bg-black text-white hover:opacity-75 duration-200">
          <p>Vente de fin d'année jusqu'à 90 % - Achetez maintenant !</p>
        </div>
      </div>
    </div>
  </div>
</div>

        <div class="mt-4">
          <div class="flex justify-between items-center px-3">
            <span class="text-xl font-semibold">Nouvelle Collection</span>
            <a href="#" class="text-green-600 text-sm">voir tout</a>
          </div>

          <div class="grid grid-cols-1 md:grid-cols-4 gap-4 p-3">
            <div class="bg-white text-black rounded-xl p-3 flex flex-col items-center">
              <img src="./assets/chaussure2.png" alt="Product 1" class="h-40 w-full object-cover rounded-lg" />
              <span> Nike Air Max 90 Futura</span>
              <span>101,97 €</span>
            </div>

            <div class="bg-white text-black rounded-xl p-3 flex flex-col items-center">
              <img src="./assets/chaussure2.png" alt="Product 1" class="h-40 w-full object-cover rounded-lg" />
              <span> Nike Air Max 90 Futura</span>
              <span>101,97 €</span>
            </div>

            <div class="bg-white text-black rounded-xl p-3 flex flex-col items-center">
              <img src="./assets/chaussure2.png" alt="Product 1" class="h-40 w-full object-cover rounded-lg" />
              <span> Nike Air Max 90 Futura</span>
              <span>101,97 €</span>
            </div>


          </div>
        </div>
      </div>
    </div>
</template>


