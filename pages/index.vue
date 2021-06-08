<template>
  <article
    class="p-10 font-sans"
    style="max-width:1000px;margin: 0px auto;"
  >
    <div class="flex justify-center">
      <div style="width:500px;">
        <img
          src="/img/gnostic-logo-mob.svg"
          style="height:100%;width:100%;"
          alt="GNOSTIC LOGIC"
        />
      </div>
    </div>
    <h1 class="font-header text-5xl py-10 text-center">
      Web development in the <span class="text-primary"> {heart}</span> of
      Scotland
    </h1>
    <div class = "pb-10">
    <h2 class="font-header text-3xl">Bespoke solutions</h2>
    <p>
      We believe there isn't a 'one size fits all' approach to web development.
      With 15+ years experience in many technologies we will work hard to find
      the exact solution for your business. We won't use off-the-shelf templates
      to design your site: the site will be crafted to meet your needs not
      someone else's.
    </p>
    </div>
    <div class = "pb-10">
    <h2 class="font-header text-3xl">Ethical development</h2>
    <ul>
      <li>Minimise environmental impact</li>
      <li>Accessible to all</li>
      <li>Respect privacy</li>
    </ul>
    </div>
  </article>
</template>

<script>
export default {
  async asyncData({ $content }) {
    const posts = await $content("blog").fetch();

    return {
      posts
    };
  },
  head() {
    return {
      title: "GNOSTIC [LOGIC]",
      meta: [
        { charset: "utf-8" },
        { name: "viewport", content: "width=device-width, initial-scale=1" },
        {
          hid: "description",
          name: "description",
          content: "Modern, innovative web development"
        }
      ],
      script: [
        { src: "https://identity.netlify.com/v1/netlify-identity-widget.js" }
      ]
    };
  }
};
</script>

<style>
body {

}
</style>
