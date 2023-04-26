<template>
  <div :id="id" class="w-full bg-[var(--app-color)] px-4 py-2 mt-4 mb-6 lg:mb-8 text-white rounded">
    <slot />
  </div>
</template>

<script>
export default {
  name: 'HeaderContent',
  props: {
    id: {
      type: String,
      default: ''
    }
  }
}
</script>
