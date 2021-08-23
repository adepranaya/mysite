<template>
  <div class="h-full flex items-center">
    <div
      class="flex justify-center md:justify-between w-full relative p-10 md:p-0"
    >
      <div class="w-auto self-center md:px-10 lg:px-20 relative z-10">
        <back-button></back-button>
        <h1 class="text-4xl md:text-6xl font-bold lg:-my-3">
          About <span class="text-cyan-400">Me</span>
        </h1>
        <div class="mt-6 grid md:grid-cols-2">
          <p>
            My name is Ade Pranaya, I graduated from Pasundan University. I am
            Web Designer / Developer. I am very happy with programming
            especially in Frontend Development so that's why right now I want to
            focus as Frontend Developer. U can check my last job
            <nuxt-link to="/portfolio" class="text-cyan-400">here</nuxt-link>
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import BackButton from "~/components/BackButton";
export default {
  components: {
    BackButton
  }
};
</script>

<style></style>
