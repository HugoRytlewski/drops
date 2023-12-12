<script setup>

let home = ref(true)
let search = ref(false)
let favorite = ref(false)
let profile = ref(false)




</script>

<template>
    <title>Drops</title>
    <nav class="flex items-center justify-between p-4 fixed top-0 left-0 right-0 bg-neutral-950 border-b border-gray-800 z-50">
      <img src="./assets/menu.svg" alt="Menu" class="h-6 w-6" />
      <h1 class="text-2xl text-white font-bold">DROPS</h1>
      <img src="./assets/panier.svg" alt="Cart" class="h-6 w-6 fill-white text-white" />
    </nav>

    <footer class="z-20 fixed inset-x-0 bottom-10 mx-auto bg-black w-56 h-14 rounded-full flex justify-around items-center">
      <div class=" rounded-full h-10 w-10 justify-center flex items-center" :class="{ 'bg-white rounded-full text-black fill-black': home }">
        <svg class="hover:opacity-75 duration-200 h-6 w-6 text-black " :class="{ 'bg-white rounded-full text-black fill-black': home }" xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px" fill="#FFFFFF"><path d="M0 0h24v24H0z" fill="none"/><path d="M10 20v-6h4v6h5v-8h3L12 3 2 12h3v8z"/></svg>

      </div>
      <div class=" rounded-full h-10 w-10 justify-center flex items-center" :class="{ 'bg-white rounded-full text-black fill-black': search }">

        <svg class="hover:opacity-75 duration-200 h-6 w-6 text-black " :class="{ 'bg-white rounded-full text-black fill-black': search }" xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px" fill="#FFFFFF"><path d="M0 0h24v24H0z" fill="none"/><path d="M15.5 14h-.79l-.28-.27C15.41 12.59 16 11.11 16 9.5 16 5.91 13.09 3 9.5 3S3 5.91 3 9.5 5.91 16 9.5 16c1.61 0 3.09-.59 4.23-1.57l.27.28v.79l5 4.99L20.49 19l-4.99-5zm-6 0C7.01 14 5 11.99 5 9.5S7.01 5 9.5 5 14 7.01 14 9.5 11.99 14 9.5 14z"/></svg>    </div>

    <div class=" rounded-full h-10 w-10 justify-center flex items-center" :class="{ 'bg-white rounded-full text-black fill-black': favorite }">

      <svg class="hover:opacity-75 duration-200 h-6 w-6 text-black " :class="{ 'bg-white rounded-full text-black fill-black': favorite }" xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px" fill="#FFFFFF"><path d="M0 0h24v24H0z" fill="none"/><path d="M12 21.35l-1.45-1.32C5.4 15.36 2 12.28 2 8.5 2 5.42 4.42 3 7.5 3c1.74 0 3.41.81 4.5 2.09C13.09 3.81 14.76 3 16.5 3 19.58 3 22 5.42 22 8.5c0 3.78-3.4 6.86-8.55 11.54L12 21.35z"/></svg>    </div>

    <div class=" rounded-full h-10 w-10 justify-center flex items-center" :class="{ 'bg-white rounded-full text-black fill-black': profile }">

      <svg class="hover:opacity-75 duration-200 h-6 w-6 text-black " :class="{ 'bg-white rounded-full text-black fill-black': profile }" xmlns="http://www.w3.org/2000/svg" enable-background="new 0 0 24 24" height="24px" viewBox="0 0 24 24" width="24px" fill="#FFFFFF"><g><rect fill="none" height="24" width="24"/></g><g><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm0 4c1.93 0 3.5 1.57 3.5 3.5S13.93 13 12 13s-3.5-1.57-3.5-3.5S10.07 6 12 6zm0 14c-2.03 0-4.43-.82-6.14-2.88C7.55 15.8 9.68 15 12 15s4.45.8 6.14 2.12C16.43 19.18 14.03 20 12 20z"/></g></svg>    </div>

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

        <div class="mt-4 bg-green-600 rounded-xl">
          <div class="flex justify-between items-center px-3">
            <span class="text-xl font-semibold mt-3">Nouvelle Collection !</span>
            <a href="#" class="text-green-600 text-sm font-bold">voir tout</a>
          </div>

          <div class="grid grid-cols-1 md:grid-cols-4 gap-4 p-3">
            <div class="bg-black text-black rounded-xl p-3 flex flex-col items-center">
              <img src="./assets/chaussure2.png" alt="Product 1" class="h-40 w-full object-cover rounded-lg" />
              <span class="text-white"> Nike Air Max 90 Futura</span>
              <span class="text-white">101,97 €</span>
            </div>

            <div class="bg-black text-black rounded-xl p-3 flex flex-col items-center">
              <img src="./assets/chaussure3.png" alt="Product 1" class="h-40 w-full object-cover rounded-lg" />
              <span class="text-white"> Nike Precision 6 </span>
              <span class="text-white">74,99 €</span>
            </div>

            <div class="bg-white text-black rounded-xl p-3 flex flex-col items-center">
              <img src="./assets/chaussure4.png" alt="Product 1" class="h-40 w-full object-cover rounded-lg" />
              <span class="text-black"> Chaussures Nike Air Max 90</span>
              <span class="text-black">160,00 €</span>
            </div>


          </div>
        </div>
      </div>
    </div>
</template>


