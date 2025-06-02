<template>
  <section
    class="h-screen flex flex-col justify-center items-center text-center bg-cover bg-center px-4"
  >
    <h1 class="text-5xl md:text-6xl font-extrabold leading-tight text-white drop-shadow-lg animate-fade-in">
      Hi, I'm Lael Mulenga
    </h1>
    <p class="mt-4 text-xl md:text-2xl text-gray-200">
      Full-Stack Web Developer specializing in building clean, performant apps.
    </p>
    <a
      href="#projects"
      class="mt-6 px-8 py-3 bg-green-500 text-white font-semibold rounded-full shadow-md hover:bg-green-600 transition duration-300"
    >
      View My Work
    </a>
  </section>
</template>

<style scoped>
@keyframes fade-in {
  from {
    opacity: 0;
    transform: translateY(20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
.animate-fade-in {
  animation: fade-in 10s ease-out;
}
</style>
