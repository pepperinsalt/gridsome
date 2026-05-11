<template>
  <section v-editable="blok" class="relative min-h-screen flex items-center justify-center bg-gray-900 overflow-hidden px-6">
    <!-- Glassmorphism Container -->
    <div class="relative z-10 max-w-4xl w-full bg-white/10 backdrop-blur-lg border border-white/20 rounded-3xl p-10 md:p-16 shadow-2xl text-center">
      <h1 class="text-5xl md:text-7xl font-extrabold text-transparent bg-clip-text bg-gradient-to-r from-blue-400 to-purple-300 mb-6">
        {{ blok.headline || "Full-Stack & Hardware Engineer" }}
      </h1>
      <p class="text-xl md:text-2xl text-gray-200 mb-8 font-light">
        {{ blok.subline || "Bridging the gap between 10 years of advanced web development, WooCommerce automation, and physical data cabling." }}
      </p>
      <div class="flex justify-center gap-4">
        <a href="#projects" class="px-8 py-3 rounded-full bg-blue-600/80 hover:bg-blue-500/90 text-white font-semibold backdrop-blur-md transition-all">
          View Projects
        </a>
        <a href="#contact" class="px-8 py-3 rounded-full bg-white/10 hover:bg-white/20 border border-white/30 text-white font-semibold backdrop-blur-md transition-all">
          Get in Touch
        </a>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  props: {
    blok: {
      type: Object,
      required: true
    }
  }
}
</script>
