<template>
  <div v-editable="blok" class="p-8 bg-white/5 backdrop-blur-md border border-gray-700 rounded-2xl shadow-lg hover:shadow-2xl transition-all duration-300 transform hover:-translate-y-2">
    <!-- Icon Placeholder -->
    <div class="h-14 w-14 bg-gradient-to-br from-blue-500 to-purple-600 rounded-xl mb-6 flex items-center justify-center shadow-inner">
      <span class="text-white font-bold text-xl">{{ blok.name ? blok.name.charAt(0) : '*' }}</span>
    </div>
    
    <h3 class="text-2xl font-bold text-gray-100 mb-3">
      {{ blok.name }}
    </h3>
    
    <p class="text-gray-400 leading-relaxed">
      {{ blok.description }}
    </p>
  </div>
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
