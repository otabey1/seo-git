<template>
  <div class="">
    <div class="text-center">
    <nuxt-logo />
    <h1>{{ title }}</h1>
    </div>
  </div>
</template>
<script>
  export default {
    name: "AboutPage",
    data() {
      return {
        title: 'my website title'
      }
    },
    head() {
      return {
        title: this.title,
        meta: [
          {
            hid: 'description',
            name: 'description',
            content: 'Otabek olimov Qamarazzamon'
          }
        ],
        script: [
          {
            src:
              'https://cdnjs.cloudflare.com/ajax/libs/jquery/3.1.1/jquery.min.js'
          }
        ],
        link: [
          {
            rel: 'stylesheet',
            href: 'https://fonts.googleapis.com/css?family=Roboto&display=swap'
          }
        ]
      }
    }
  }
</script>
<style scoped>
  h1 {
    font-family: Roboto, sans-serif;
  }
</style>