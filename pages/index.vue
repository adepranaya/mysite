<template>
  <div class="h-full flex items-center">
    <div
      class="flex justify-center md:justify-between w-full relative p-10 md:p-0"
    >
      <div class="w-auto self-center md:pl-10 lg:pl-20 relative z-10">
        <div class="text-xl md:text-4xl">Hi, I’m</div>
        <h1 class="text-4xl md:text-6xl font-bold lg:-my-3">
          A<span class="text-cyan-400">dePran</span>aya
        </h1>
        <div class="text-xl md:text-4xl mb-2">web designer/developer</div>
        <div class="mt-4 grid grid-cols-1 md:grid-cols-2 gap-4">
          <a
            class="bg-cyan-400 text-white font-semibold py-2 px-4 border-2 border-transparent hover:bg-gray-900 hover:border-transparent rounded-full flex-1 uppercase sm:mb-0 sm:mr-2 text-center cursor-pointer"
            href="mailto:adepranaya@gmail.com"
            >contact me</a
          >
          <!-- href="mailto:adepranaya@gmail.com?subject=I want hire you!&body=Hello Ade!, my name is ..." -->
          <nuxt-link
            to="/about"
            class="bg-transparent text-cyan-700 font-semibold border-2 border-cyan-700 hover:text-white hover:bg-gray-900 hover:border-transparent py-2 px-4 rounded-full sm:flex-1 uppercase text-center"
            >about</nuxt-link
          >
          <nuxt-link
            to="/portfolio"
            class="bg-transparent text-cyan-700 font-semibold border-2 border-cyan-700 hover:text-white hover:bg-gray-900 hover:border-transparent py-2 px-4 rounded-full sm:flex-1 uppercase text-center sm:col-span-2"
            >see my works</nuxt-link
          >
        </div>
      </div>
      <img
        src="~/assets/img/depran_transaparent.png"
        alt
        class="hidden md:inline-block w-0 md:w-0 lg:w-5/12 xl:w-1/3 md:pr-10 lg:pr-20 self-end"
      />
    </div>
      <img
        src="~/assets/img/wave_right_bottom.svg"
        alt
        class="hidden lg:inline-block absolute z-1 w-2/5 bottom-0 right-0"
      />
  </div>
</template>

<script>

export default {
};
</script>
