<script setup>

let home = ref(false)
let search = ref(true)
let favorite = ref(false)
let profile = ref(false)




</script>

<template>
       <nav class="flex items-center justify-between p-4 fixed top-0 left-0 right-0 bg-neutral-950 border-b border-gray-800 z-50">
      <svg class="text-white fill-white h-6 w-6 cursor-pointer" xmlns="http://www.w3.org/2000/svg" height="24" viewBox="0 -960 960 960" width="24"><path d="M360-240 120-480l240-240 56 56-144 144h568v80H272l144 144-56 56Z"/></svg>
      <div class="flex gap-2 h-10 items-center justify-center overflow-hidden">
        <h1 class="text-2xl text-white font-bold cursor-pointer">DROPS</h1>

      </div>
      <img src="../assets/panier.svg" alt="Cart" class="h-6 w-6 fill-white text-white cursor-pointer " />
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
    <div class="z-0 flex flex-col  md:items-center min-h-screen bg-neutral-950 text-white">
        <div class="pt-16 pb-4 px-4 mt-20">
            <div class="gap-8 flex flex-col">

            <div class="rounded-xl  h-64 bg-white overflow-hidden flex items-center justify-center ">
                <img class="object-cover" src="../assets/chaussure.png" alt="">
            </div>
            <div class="flex w-full justify-left gap-6 ">
                <div class="h-16 bg-white rounded-xl overflow-hidden  border-4 border-green-600 flex items-center justify-center">
                    <img class="object-cover h-14" src="../assets/chaussure.png" alt="">
                </div>
                <div class="h-16 bg-white rounded-xl overflow-hidden   flex items-center justify-center">
                    <img class="object-cover h-14" src="../assets/chaussure2.png" alt="">
                </div>
                <div class="h-16 bg-white rounded-xl overflow-hidden   flex items-center justify-center">
                    <img class="object-cover h-14" src="../assets/chaussure.png" alt="">
                </div>

                
                
            </div>
           

        </div>
        <div class="flex flex-col mt-6 gap-6 bg-green-600 rounded-xl p-3    ">
            <span class="text-white text-xl font-bold"> Nike Air Max 90 Futura</span>
            <span class="text-white font-bold text-xl">101,97 €</span>
            <span class="font-bold">Taille :</span>

            <div class="flex  gap-2">
                <div class="h-10 w-10 bg-white rounded-full flex items-center justify-center"><p class="text-green-600 font-bold">38</p></div>
                <div class="h-10 w-10 bg-white rounded-full flex items-center justify-center"><p class="text-green-600 font-bold">39</p></div>
                <div class="h-10 w-10 bg-white rounded-full flex items-center justify-center"><p class="text-green-600 font-bold">40</p></div>
                <div class="h-10 w-10 bg-white rounded-full flex items-center justify-center"><p class="text-green-600 font-bold">41</p></div>
                <div class="h-10 w-10 bg-white rounded-full flex items-center justify-center"><p class="text-green-600 font-bold">42</p></div>
                <div class="h-10 w-10 bg-white rounded-full flex items-center justify-center"><p class="text-green-600 font-bold">43</p></div>

           
            </div>
            <div class="bg-white rounded-xl flex items-center p-2 justify-center w-20 ">
                <p class="text-green-600 ">Acheter</p>
            </div>
            <div class="bg-green-600 rounded-xl flex items-center justify-center w-fit border border-white p-2 ">
                <p>Mettre dans le panier</p>
            </div>
        </div>
     

    </div>


</div>

<div class="h-96 bg-neutral-950">

</div>
</template>