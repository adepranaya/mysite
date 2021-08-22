<template>
  <div class="tracking-widest flex justify-center bg-gray-400">
    <div
      class="min-400 h-screen w-screen max-w-screen-xl relative bg-white shadow-lg"
    >
      <img
        src="~/assets/img/ellipse.svg"
        alt
        class="hidden md:inline-block absolute z-0 top-0 right-0 w-1/3"
      />
      <div class="w-full inline-block h-full flex flex-col">
        <nav class="hidden md:block mx-10 lg:mx-20 py-6">
          <ul class="flex uppercase">
            <li class="mr-6">
              <nuxt-link to="/" class="text-gray-900 hover:text-teal-800"
                >home</nuxt-link
              >
            </li>
            <li class="mr-6">
              <nuxt-link to="/about" class="text-gray-900 hover:text-teal-800"
                >about me</nuxt-link
              >
            </li>
            <li class="mr-6">
              <nuxt-link
                to="/portfolio"
                class="text-gray-900 hover:text-teal-800"
                >portfolio</nuxt-link
              >
            </li>
            <li class="mr-6 hidden">
              <a class="text-gray-900 hover:text-teal-800" href="#">skills</a>
            </li>
            <li class="mr-6">
              <a
                class="text-gray-900 hover:text-teal-800"
                href="mailto:adepranaya@gmail.com?subject=I want hire you!&body=Hello Ade!, my name is ..."
                >contact</a
              >
            </li>
          </ul>
        </nav>
        <nuxt />
        <div class="py-1 px-10 lg:px-20 w-full relative z-2">
          <div class="mt-4 flex items-center mb-4">
            <a
              href="https://instagram.com/depran7"
              target="_blank"
              class="mr-5"
            >
              <img src="~/assets/img/instagram_icon.svg" alt class="h-10" />
            </a>
            <a
              href="https://www.youtube.com/channel/UCNEqtGZAM-LiBeSATMrOvVQ?sub_confirmation=1"
              target="_blank"
              class="mr-5"
            >
              <img src="~/assets/img/youtube_icon.svg" alt class="h-10" />
            </a>
            <span>copyright &copy; {{ currentDate }}. {{ name }}</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      currentDate: new Date().getFullYear().toString(),
      name: "Ade Pranaya"
    };
  }
};
</script>
<style>
body {
  font-family: "Montserrat";
}
</style>
