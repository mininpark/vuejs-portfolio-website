<template>
  <header>
    <h1><a v-bind:href="'/Home'">Poka</a></h1>
  </header>
</template>

<script>

export default {
  name: 'Header',
  props: {
    title: String,
  },
  components: {
  },
}
</script>

<style lang="scss">

</style>