<template>
  <section id="projects" class="py-20 px-6 bg-gray-900 text-white text-center">
    <h2 class="text-4xl font-bold mb-10">Projects</h2>
    <div class="grid gap-8 md:grid-cols-2 lg:grid-cols-3 max-w-6xl mx-auto">
      <div
        v-for="project in projects"
        :key="project.title"
        class="bg-gray-800 rounded-2xl shadow-lg p-6 transition-transform transform hover:-translate-y-2 hover:shadow-2xl"
      >
        <h3 class="text-2xl font-semibold mb-2">{{ project.title }}</h3>
        <p class="text-gray-300 mb-4">{{ project.description }}</p>
        <a
          :href="project.link"
          target="_blank"
          class="inline-block mt-auto text-green-400 hover:underline"
        >
          View Project →
        </a>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      projects: [
        {
          title: "Portfolio Website",
          description:
            "A sleek personal portfolio built with Vue.js and Tailwind CSS.",
          link: "#", //add a link to the portfolio website
        },
        {
          title: "Hospital Management System",
          description:
            "A full-stack web app for managing hospital records and lab results.",
          link: "#", //add a link to the hospital management system 
        },
        {
          title: "E-Commerce Dashboard",
          description:
            "Admin dashboard for tracking orders, users, and product analytics.",
          link: "#", //add a link to the E-commerce website
        },
      ],
    };
  },
};
</script>
