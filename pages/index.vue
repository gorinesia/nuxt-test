<template>
  <div>
    index<br />
    <NuxtLink to="/about">about</NuxtLink>
    <Logo />
    <BaseHeader />
  </div>
</template>

<script>
export default {
  asyncData() {
    console.log('asyncData')
  },
  fetch(context) {
    console.log(context.route.name)
    console.log('fetch')
  },
  created() {
    console.log('created')
  },
}
</script>

<style>
</style>
