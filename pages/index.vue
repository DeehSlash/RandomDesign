<template>
  <section class="container">
    <div>
      <app-logo/>
      <h1 class="title">
        random-design
      </h1>
      <h2 class="subtitle">
        Random Design
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

<style>
  .container {
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
  }
</style>

<script>
  export default {
    components: {
      AppLogo
    }
  }
</script>
