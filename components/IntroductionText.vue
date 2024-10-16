<template>
        <div class="text-4xl sm:text-5xl md:text-7xl lg:text-9xl">ACHECHE Achraf</div>
        <div class="textdisplay text-3xl sm:text-4xl md:text-6xl lg:text-8xl h-[10vh]">{{ displayedText }}</div>
        <div class="flex flex-row mt-[3vh]">
          <Icon name="uil:github" class="w-[3vw] h-[4vh]" />
          <Icon name="uil:facebook" class="w-[3vw] h-[4vh]" />
          <Icon name="uil:twitter" class="w-[3vw] h-[4vh]" />
          <Icon name="uil:linkedin" class="w-[3vw] h-[4vh]" />
          <Icon name="uil:youtube" class="w-[3vw] h-[4vh]" />
        </div>
        
</template>


<script lang="ts" setup>
import { ref, onMounted } from 'vue';

const phrases = ref(['E-health Engineering Student', 'Web Developer']);
let phraseIndex = 0; 

const displayedText = ref(''); 
const typingSpeed = 60; 
const pauseBetweenPhrases = 3000; 
const deleteSpeed = 60; 

// Function to type out the text
const typeText = () => {
  let index = 0;
  displayedText.value = ''; 

  const interval = setInterval(() => {
    if (index < phrases.value[phraseIndex].length) {
      displayedText.value += phrases.value[phraseIndex][index]; 
      index++;
    } else {
      clearInterval(interval); 
      setTimeout(deleteText, pauseBetweenPhrases); 
    }
  }, typingSpeed);
};

// Function to delete the text character by character
const deleteText = () => {
  let index = displayedText.value.length;

  const interval = setInterval(() => {
    if (index > 0) {
      displayedText.value = displayedText.value.slice(0, index - 1); 
      index--;
    } else {
      clearInterval(interval); 
      setTimeout(swapPhrase, pauseBetweenPhrases); 
    }
  }, deleteSpeed);
};


const swapPhrase = () => {
  phraseIndex = (phraseIndex + 1) % phrases.value.length; 
  typeText(); 
};


onMounted(() => {
  typeText(); 
});

</script>

<style scoped>
.textdisplay:after {
  content: "|";
  animation: blink 1s step-end infinite;
}

@keyframes blink {
  from, to {
    opacity: 0;
  }
  50% {
    opacity: 1;
  }
}
</style>
