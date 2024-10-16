<template>
    <div class="flex flex-col md:flex-row h-full w-full justify-center items-center">
        <div class="flex flex-col basis-1/4 justify-center items-center h-full w-full fonnt-semibold ">
          <div
            class="justify-center items-center text-2xl sm:text-3xl md:text-4xl lg:text-5xl font-serif font-bold mb-[5vh] ">
            Contact Me</div>
          <div class="flex flex-row gap-[1vw] justify-left items-center w-[39vh] ">
            <Icon name="f7:envelope-fill" class="w-[3vw] h-[4vh]" />
            <div class=" h-[4vh] mt-[0.90vh]">achecheachraf@gmail.com</div>
          </div>
          <div class="flex flex-row gap-[1vw] justify-left items-center w-[39vh] ">
            <Icon name="uil:phone" class="w-[3vw] h-[4vh]" />
            <div class=" h-[4vh] mt-[0.90vh]">+33 074565656</div>
          </div>
          <div class="flex flex-row gap-[1vw] justify-left items-center w-[39vh] ">
            <Icon name="uil:linkedin" class="w-[3vw] h-[4vh]" />
            <div class=" h-[4vh] mt-[0.90vh]">
              <a href="https://fr.linkedin.com/in/achecheachraf" target="_blank" class="hover:text-sky-500 underline">
                achecheachraf
              </a>
            </div>
          </div>

        </div>
        <div class="flex flex-col basis-1/2  justify-center items-center  gap-[4vh]">
          <div class=" text-2xl sm:text-3xl md:text-4xl lg:text-5xl font-serif font-bold mb-[5vh] ">Send me a Message
          </div>
          <div class="flex flex-row justify-start items-center gap-[2vw] ">
            <input type="text" placeholder="Name"
              class="placeholder:font-serif placeholder:text-lg border-1 shadow-lg w-[17vw] border-b-2 h-[4vh] border-slate-700 dark:border-pink-50 bg-pink-50 dark:bg-slate-950">
            <input type="text" placeholder="Phone"
              class="placeholder:font-serif placeholder:text-lg border-1 shadow-lg w-[17vw] border-b-2 h-[4vh] border-slate-700 dark:border-pink-50 bg-pink-50 dark:bg-slate-950">
          </div>

          <div class="flex flex-row justify-start items-center gap-[2vw] b">
            <input type="text" placeholder="Email"
              class="placeholder:font-serif placeholder:text-lg border-1 shadow-lg w-[17vw] border-b-2 h-[4vh] border-slate-700 dark:border-pink-50 bg-pink-50 dark:bg-slate-950">
            <input type="text" placeholder="Subject"
              class="placeholder:font-serif placeholder:text-lg border-1 shadow-lg w-[17vw] border-b-2 h-[4vh] border-slate-700 dark:border-pink-50 bg-pink-50 dark:bg-slate-950">
          </div>

          <textarea placeholder="Text"
            class="placeholder:font-serif placeholder:text-lg border-1 shadow-lg w-[36vw] h-[12vh] border-b-2 border-slate-700 dark:border-pink-50 bg-pink-50 dark:bg-slate-950 placeholder:text-left placeholder:pt-2"></textarea>
          <div class="flex flex-row justify-start items-center  w-full">
              <button class="font-bold underline underline-offset-2 decoration-2 ml-[10vw]">SEND MESSAGE</button>
          </div>
        </div>

      </div>
</template>