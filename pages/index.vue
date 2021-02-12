<template>
  <section class="container">
    <div>
      <logo/>
      <h1 class="title">
        nuxtwindify
      </h1>
      <h2 class="subtitle">
        Nuxt - Tailwind - Netlify starter
      </h2>
      <div class="links">
        <a
          href="https://nuxtjs.org/"
          target="_blank"
          class="button--green">Documentation</a>
        <a
          href="https://github.com/nuxt/nuxt.js"
          target="_blank"
          class="button--grey">GitHub</a>
      </div>
    </div>
  </section>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  // Netlify script to identify user
  head() {
    return {
      script: [
        { src: 'https://identity.netlify.com/v1/netlify-identity-widget.js' }
      ]
    }
  },
  components: {
    Logo
  }
}
</script>
