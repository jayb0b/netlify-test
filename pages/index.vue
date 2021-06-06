<template>
<article class = "p-10 font-sans" style ="max-width:1000px;margin: 0px auto;">
    <div class = "flex justify-center	">
   <img src="/img/gnostic-logo.svg"  style="max-width:500px;" alt = "GNOSTIC LOGIC" />
    </div>
  <h1 class = "font-header text-5xl py-10 text-center">Web development in the heart of Scotland</h1>
  <h2 class = "font-header text-3xl">Bespoke solutions</h2>
  <p>We believe there isn't a 'one size fits all' approach to web development. With 15+ years experience in many technologies we will work hard to find the exact solution for your business. We won't use off-the-shelf templates to design your site: the site will be crafted to meet your needs not someone else's.</p>
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
  body{
    color:#3B3D3F;
  }
</style>
