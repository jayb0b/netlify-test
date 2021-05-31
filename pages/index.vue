<template>
<article>
  <section class = "flex justify-center">
  <img class ="mx-auto" style = "display:block;max-width:100%;" src = "/img/gnostic-logo.svg" alt="Gnostic Logic"/>
  </section>
</article>
</template>

<script>
export default {
     async asyncData({ $content }) {
    const posts = await $content("blog").fetch();

    return {
      posts,
    };
  },
  head() {
    return {
      title: "GNOSTIC [LOGIC]",
          meta: [
      { charset: 'utf-8' },
      { name: 'viewport', content: 'width=device-width, initial-scale=1' },
      { hid: 'description', name: 'description', content: 'Modern, innovative web development' }
    ],
      script: [{ src: 'https://identity.netlify.com/v1/netlify-identity-widget.js' }],
    };
  },
};
</script>

<style>

</style>
