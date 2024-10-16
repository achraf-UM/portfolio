<template>
<nav class="sticky top-0 left-0 right-0 z-50 flex flex-row shadow-lg backdrop-blur-sm bg-white/50 dark:bg-slate-800/50 h-[8vh] items-center  justify-center w-screen gap-2">
    <div class="basis-1/2 flex justify-start items-center text-[4vw] font-serif text-black dark:text-white ml-[7vw]"><a>ⱯA</a></div>
    <ul class="basis-1/2  flex justify-end items-center flex-row mr-[7vw]">
        <li class="text-[2vw]  text-black dark:text-white"><button @click="toggleDarkMode">
          <Icon name="line-md:moon-filled-alt-loop" class="w-[3vw] h-[4vh]" />
        </button></li>
    </ul>
</nav>
</template>

<script setup>
    const isDark = ref(false);

const toggleDarkMode = () => {
  isDark.value = !isDark.value;
  const htmlEl = document.documentElement;
  if (isDark.value) {
    htmlEl.classList.add('dark');
  } else {
    htmlEl.classList.remove('dark');
  }
};
</script>