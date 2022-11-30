<template>
      <div>
        <NavBar uk-sticky="show-on-up: true"/>
        <Nuxt />
        <MainFooter />
      </div>
</template>

<script>
export default {
  name: 'DefaultLayout',
  data() {
    return {
      clipped: false,
      active: false
    }
  },
}
</script>
<style>
</style>
