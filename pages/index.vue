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
  asyncData({ route, isDev, app, $axios }) {
    console.log('asyncData')
    console.log('route.name:', route.name)
    console.log('isDev:', isDev)
    console.log('app:', app)
    console.log('app.$axios:', app.$axios)
    console.log('$axios:', $axios)
    console.log('======================')
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
