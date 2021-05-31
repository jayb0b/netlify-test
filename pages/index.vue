<template>
<article>
  <section class = "flex  justify-center">
  <img class ="p-4 max-w-3xl mx-auto" src = "/img/gnostic-logo.svg" alt="Gnostic Logic"/>
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
      script: [{ src: 'https://identity.netlify.com/v1/netlify-identity-widget.js' }],
    };
  },
};
</script>

<style>

</style>
