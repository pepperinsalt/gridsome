<template>
  <div v-editable="blok" class="w-full">
    <component
      v-for="item in blok.body"
      :key="item._uid"
      :blok="item"
      :is="item.component"
    />
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
