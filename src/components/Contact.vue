<template>
  <section id="contact" class="py-20 px-6 bg-gray-900 text-white text-center">
    <h2 class="text-4xl font-bold mb-10">Get in Touch</h2>
    <form
      @submit.prevent="submitForm"
      class="max-w-2xl mx-auto bg-gray-800 p-8 rounded-2xl shadow-lg space-y-6"
    >
      <input
        v-model="form.name"
        type="text"
        placeholder="Your Name"
        class="w-full px-4 py-3 rounded-lg bg-gray-700 text-white focus:outline-none focus:ring-2 focus:ring-green-500"
        required
      />
      <input
        v-model="form.email"
        type="email"
        placeholder="Your Email"
        class="w-full px-4 py-3 rounded-lg bg-gray-700 text-white focus:outline-none focus:ring-2 focus:ring-green-500"
        required
      />
      <textarea
        v-model="form.message"
        rows="5"
        placeholder="Your Message"
        class="w-full px-4 py-3 rounded-lg bg-gray-700 text-white focus:outline-none focus:ring-2 focus:ring-green-500"
        required
      ></textarea>
      <button
        type="submit"
        class="w-full bg-green-500 hover:bg-green-600 text-white font-semibold py-3 px-6 rounded-lg transition duration-300"
      >
        Send Message
      </button>
    </form>
    <p v-if="submitted" class="mt-6 text-green-400 font-medium">
      Thanks! Your message has been sent.
    </p>
  </section>
</template>

<script>
export default {
  data() {
    return {
      form: {
        name: "",
        email: "",
        message: "",
      },
      submitted: false,
    };
  },
  methods: {
    submitForm() {
      // Simulate form submission — you can replace this with a real API later
      console.log("Form submitted:", this.form);
      this.submitted = true;
      this.form = { name: "", email: "", message: "" };
    },
  },
};
</script>
