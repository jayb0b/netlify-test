<template>
  <main class="font-sans container mx-auto">
    <article class = "px-10 md:px-0">
    <section class = "indented pb-64 px-10 -mx-10 md:mx-0 md:px-0" style = "background-image: url(/img/texture.svg);">
    <header class="flex justify-center" style = "" >
      <div style="width:500px;" >
        <img
          src="/img/gnostic-logo-mob.svg"
          style="height:100%;width:100%;"
          alt="GNOSTIC LOGIC"
        />
      </div>
    </header>
    <h1 class="font-header text-6xl py-10 text-center">
      Web development in the <span class="text-primary"> {heart}</span> of
      Scotland
    </h1>
    </section>
    <div class="-mt-64 md:grid grid-cols-3 gap-10" style = " background-image: linear-gradient(to bottom, rgba(244,247,240,0), rgba(244,247,240,1)); ">
      <div class="p-10 rounded-md mb-10" style = "background-color:#2c7169;color:white;">
        <h2 class="font-header text-4xl pb-2">Bespoke solutions</h2>
        <p class = "text-white">
          We believe there isn't a 'one size fits all' approach to web
          development. With 15+ years experience in many technologies we will
          work hard to find the exact solution for your business. We won't use
          off-the-shelf templates to design your site: the site will be crafted
          to meet your needs not someone else's.
        </p>
      </div>
            <div class="p-10 rounded-md mb-10" style = "background-color:#2c7169;color:white;">
        <h2 class="font-header text-4xl pb-2">Bespoke solutions</h2>
        <p class = "text-white">
          We believe there isn't a 'one size fits all' approach to web
          development. With 15+ years experience in many technologies we will
          work hard to find the exact solution for your business. We won't use
          off-the-shelf templates to design your site: the site will be crafted
          to meet your needs not someone else's.
        </p>
      </div>
            <div class="p-10 rounded-md mb-10" style = "background-color:#2c7169;color:white;">
        <h2 class="font-header text-4xl pb-2">Bespoke solutions</h2>
        <p class = "text-white">
        <ul>
          <li>Minimise environmental impact</li>
          <li>Accessible to all</li>
          <li>Respect privacy</li>
        </ul>
        <button class="btn">More</button>
        </p>
      </div>
    </div>
    </article>
  </main>
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
