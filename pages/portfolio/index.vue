<template>
  <div class="tracking-widest flex justify-center bg-cyan-400">
    <div class="min-400 h-screen w-screen max-w-screen-xl relative bg-white shadow-lg">
      <div class="py-6 w-full inline-block h-full absolute z-1">
        <nav class="hidden md:inline-block mx-10 lg:mx-20">
          <ul class="flex uppercase">
            <li class="mr-6">
              <nuxt-link to="/" class="text-gray-900 hover:text-teal-800">home</nuxt-link>
            </li>
            <li class="mr-6">
              <nuxt-link to="/about" class="text-gray-900 hover:text-teal-800">about me</nuxt-link>
            </li>
            <li class="mr-6">
              <nuxt-link to="/portfolio" class="text-cyan-400 font-bold">portfolio</nuxt-link>
            </li>
            <li class="mr-6 hidden">
              <a class="text-gray-900 hover:text-teal-800" href="#">skills</a>
            </li>
            <li class="mr-6">
              <a
                class="text-gray-900 hover:text-teal-800"
                href="mailto:adepranaya@gmail.com?subject=I want hire you!&body=Hello Ade!, my name is ..."
              >contact</a>
            </li>
          </ul>
        </nav>
        <div class="h-full flex items-center">
          <div class="flex justify-center md:justify-between w-full relative p-10 md:p-0">
            <div class="w-auto self-center md:px-10 lg:px-20 relative z-10">
                <h1 class="font-bold">Comming soon</h1>
            </div>
          </div>
        </div>
        <div class="absolute z-1 bottom-0 py-1 px-10 lg:px-20 w-full">
          <div class="mt-4 flex items-center mb-4">
            <a href="https://instagram.com/depran7" target="_blank" class="mr-5">
              <img src="~/assets/img/instagram_icon.svg" alt class="h-10" />
            </a>
            <a
              href="https://www.youtube.com/channel/UCNEqtGZAM-LiBeSATMrOvVQ?sub_confirmation=1"
              target="_blank"
              class="mr-5"
            >
              <img src="~/assets/img/youtube_icon.svg" alt class="h-10" />
            </a>
            <span>copyright &copy; {{currentDate}}. {{name}}</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Logo from "~/components/Logo.vue";

export default {
  components: {
    Logo
  },
  data() {
    return {
      currentDate: new Date().getFullYear().toString(),
      name: "Ade Pranaya"
    };
  }
};
</script>

<style>
</style>
