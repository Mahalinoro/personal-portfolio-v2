<template>
  <div>
    <Navbar/>
    <Nuxt />
  </div>
</template>

<script>
  import Navbar from '@/components/Navbar'
  export default {
    components: {
      Navbar
    },

    head: {
    titleTemplate: '%s - hello!',
    meta: [
      { charset: 'utf-8' },
      { name: 'viewport', content: 'width=device-width, initial-scale=1' }      
    ]
  }
}

  
</script>

<style lang='scss'>

html, body {
  font-family: 'Open Sans', sans-serif;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}
</style>
