<template>
  <section class="py-20 px-6 bg-gray-800 text-white text-center">
    <h2 class="text-4xl font-bold mb-10">Skills</h2>
    <div class="flex flex-wrap justify-center gap-4 max-w-4xl mx-auto">
      <span
        v-for="skill in skills"
        :key="skill"
        class="bg-gray-700 text-white px-5 py-2 rounded-full shadow hover:bg-green-500 hover:text-white transition duration-300"
      >
        {{ skill }}
      </span>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      skills: [
        "Vue.js",
        "JavaScript",
        "Node.js",
        "Java",
        "C++",
        "PHP",
        "C Language",
        "MySqlDB",
        "Tailwind CSS",
        "Git",
        "REST APIs",
        "HTML & CSS",
        "Computer Hardware and Software Repair",
        "Computer Networking",
        "Microsoft Office",
        "CCTV Installation",
      ],
    };
  },
};
</script>
