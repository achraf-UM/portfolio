<template>
  
  <div class="dark:bg-[url('/assets/bg-cloud-dark.jpg')]  w-screen   bg-[url('/assets/bg-cloud-white.png')] dark:text-white text-black">
    <TopNavBar ></TopNavBar>
    <NuxtRouteAnnouncer />
    
    <div id="section1" class="flex overflow-hidden flex-col justify-center items-center dark:bg-[url('/assets/bg-cloud-dark.jpg')] h-screen w-screen bg-cover bg-center bg-[url('/assets/bg-cloud-white.png')] dark:text-white text-black">
      
      <div class="flex flex-col justify-center items-center w-full h-full font-serif">
        
     <IntroductionText> </IntroductionText>
     
     
    </div>
  </div>


  <div id="section2" class="flex flex-col sm:flex-row justify-center items-center bg-pink-50 h-screen w-screen bg-cover bg-center dark:bg-slate-950 ">
    <div class="w-[45vh] order-first sm:order-last"><img class="basis-1/3 rounded object-cover h-auto w-auto" src="./assets/achraf.png"></div>
    <div class="basis-1/3 justify-center order-last sm:order-first font-serif text-lg sm:text-xl md:text-2xl lg:text-3xl  "><h1 class="font-bold">Hello World</h1>Lorem ipsum dolor sit amet esse culpa odit at, eum suscipit aut voluptatibus nihil sed itaque necessitatibus quaerat perspiciatis, laudantium aperiam neque fuga.</div>
    
    
    </div>
    <div id="section3" class="flex flex-col justify-center items-center bg-pink-50 h-screen w-screen dark:bg-slate-950">
      <p class="text-3xl sm:text-4xl md:text-5xl lg:text-6xl">Projects</p>
    <div  class="grid gid-cols-1 gap-2 sm:grid-cols-2 md:grid-cols-3 justify-center w-full h-[75vh]">
    <div class="flex justify-center items-center rounded-lg bg-zinc-200 w-[20vw] my-[5vh] mx-[5vw]"><img class="rounded w-[17vw]" src="./assets/shwhite.png"></div>
    <div class="flex justify-center items-center rounded-lg bg-zinc-200 w-[20vw] my-[5vh] mx-[5vw]"><img class="rounded w-[17vw]" src="./assets/shdark.png"></div> 
    <div class="flex justify-center items-center rounded-lg bg-zinc-200 w-[20vw] my-[5vh] mx-[5vw]"><img class="rounded w-[17vw]" src="./assets/shwhite.png"></div>
    <div class="flex justify-center items-center rounded-lg bg-zinc-200 w-[20vw] my-[5vh] mx-[5vw]"><img class="rounded w-[17vw]" src="./assets/shdark.png"></div>
    <div class="flex justify-center items-center rounded-lg bg-zinc-200 w-[20vw] my-[5vh] mx-[5vw]"><img class="rounded w-[17vw]" src="./assets/shwhite.png"></div> 
    <div class="flex justify-center items-center rounded-lg bg-zinc-200 w-[20vw] my-[5vh] mx-[5vw]"><img class="rounded w-[17vw]" src="./assets/shdark.png"></div>
    </div>
  </div>
  </div>

  
</template>

<script lang="ts" setup>



</script>

<style scoped>

</style>
