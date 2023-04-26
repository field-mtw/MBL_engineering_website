<template>
  <div class="mx-auto w-full max-w-screen-xl p-4 py-6 lg:py-8">
    <button class="mx-2 my-1 p-2 bg-[var(--app-color)] text-white rounded hover:underline">
      <nuxt-link to="/#machine" class="">
        Back
      </nuxt-link>
    </button>
    <MachineB v-if="routeName === 'machine-01'" />
    <MachineC v-if="routeName === 'machine-02'" />
    <MachineD v-if="routeName === 'machine-03'" />
    <MachineF v-if="routeName === 'machine-04'" />
    <MachineG v-if="routeName === 'machine-05'" />
    <MachineH v-if="routeName === 'machine-06'" />
  </div>
</template>

<script>
export default {
  name: 'ContentsView',
  data () {
    return {
      routeName: ''
    }
  },
  mounted () {
    this.routeName = this.$route.params.id
  }
}
</script>
