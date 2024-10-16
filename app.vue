<template>

  <div
    class="dark:bg-[url('/assets/bg-cloud-dark.jpg')]  w-screen   bg-[url('/assets/bg-cloud-white.png')] dark:text-white text-black">
    <TopNavBar></TopNavBar>
    <NuxtRouteAnnouncer />

    <section id="section1"
      class="flex overflow-hidden flex-col justify-center items-center dark:bg-[url('/assets/bg-cloud-dark.jpg')] min-h-screen h-auto w-screen bg-cover bg-center bg-[url('/assets/bg-cloud-white.png')] dark:text-white text-black">

      <div class="flex flex-col justify-center items-center w-full h-full font-serif">

        <IntroductionText> </IntroductionText>


      </div>
    </section>



    <section id="section2"
      class="flex flex-col sm:flex-row justify-center items-center min-h-screen h-auto w-screen bg-cover bg-center  ">
      <IntroductionPersonne></IntroductionPersonne>
    </section>

    <section id="section3" class="flex flex-col justify-center items-center min-h-screen h-auto w-screen">
      <Skills />

    </section>

    <section id="section4"
      class="flex flex-col justify-center items-center  bg-pink-50 min-h-screen h-auto w-screen dark:bg-slate-950">
      <Projects></Projects>
    </section>

    <section id="section4"
      class="flex flex-col justify-center items-center  bg-pink-50 h-screen  w-screen dark:bg-slate-950">
      <Contact></Contact>
    </section>
  </div>


</template>

<script lang="ts" setup>
const handleScroll = (event: WheelEvent) => {
  event.preventDefault(); // Prevent default scroll behavior
  const sections = document.querySelectorAll('section');
  let currentSection = Math.round(window.scrollY / window.innerHeight);

  // Handle scroll up
  if (event.deltaY < 0 && currentSection > 0) {
    window.scrollTo({
      top: (currentSection - 1) * window.innerHeight,
      behavior: 'smooth',
    });
  }
  // Handle scroll down
  else if (event.deltaY > 0 && currentSection < sections.length - 1) {
    window.scrollTo({
      top: (currentSection + 1) * window.innerHeight,
      behavior: 'smooth',
    });
  }
};

onMounted(() => {
  window.addEventListener('wheel', handleScroll, { passive: false });
});


</script>

<style scoped></style>
