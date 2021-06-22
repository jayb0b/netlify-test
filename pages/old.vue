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
    <h1 class="font-serif text-6xl py-10 text-center">
      Web development in the <span class="text-primary"> {heart}</span> of
      Scotland
    </h1>
    </section>
    <div class="-mt-64 md:grid grid-cols-3 gap-10" style = " background-image: linear-gradient(to bottom, rgba(244,247,240,0), rgba(244,247,240,1)); ">
      <div class="p-10 rounded-md h-full" style = "background-color:#2c7169;color:white;">
        <h2 class="font-header text-4xl pb-2">Bespoke solutions</h2>
        <p class = "text-white">
          We believe there isn't a 'one size fits all' approach to web
          development. We won't use
          off-the-shelf templates to design your site: the site will be crafted
          to meet your needs not someone else's.
        </p>
      </div>
            <div class="p-10 rounded-md h-full" style = "background-color:#2c7169;color:white;">
        <h2 class="font-header text-4xl pb-2">Full stack development</h2>
        <p class = "text-white">
            We have 15+ years experience developing websites.
        </p>
      </div>
            <div class="p-10 rounded-md  h-full" style = "background-color:#2c7169;color:white;">
        <h2 class="font-header text-4xl pb-2">Ethical development</h2>
        <p class = "text-white">
        <ul>
          <li>Minimise environmental impact</li>
          <li>Accessible to all</li>
          <li>Respect privacy</li>
        </ul>
        <button class="btn">Find out more</button>
        </p>
      </div>
    </div>

    <section class = "indented">
      <div class = "max-w-3xl mx-auto py-10 px-10 text-lg">
      
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Morbi id ligula venenatis, eleifend justo vitae, blandit lacus. Suspendisse risus erat, rutrum fringilla libero suscipit, eleifend convallis metus. Morbi sed augue aliquet, luctus augue at, lobortis augue. Vestibulum nec elit quis erat tristique vehicula eget vel ante. Curabitur eleifend augue in mi mollis, nec gravida ipsum sollicitudin. Phasellus nibh eros, tincidunt sed fringilla vitae, interdum volutpat lacus. Morbi lacus sapien, pellentesque vel lacus in, scelerisque laoreet erat.
</p>
<p>
Nulla facilisi. Duis iaculis suscipit nunc a auctor. Nam vestibulum augue at ligula congue, cursus congue purus dictum. Curabitur dapibus, magna ut pellentesque consequat, elit velit cursus nulla, at ornare est odio quis massa. Morbi at mi sit amet elit pharetra feugiat eu ac purus. Sed ac tempor justo, quis vehicula libero. Sed et orci elit. Nullam justo diam, ultricies et diam in, sagittis suscipit magna. Aliquam vel commodo lorem. Integer diam elit, faucibus fringilla pulvinar auctor, gravida sit amet tortor. Etiam varius sodales consectetur. Sed placerat feugiat orci, ut maximus nisi molestie eget. Nullam cursus ultrices nibh et fringilla. Donec id tellus imperdiet, molestie tellus eu, interdum turpis. Nulla commodo sodales lacinia. Etiam ut pellentesque dolor, vel placerat urna.
</p>
<p>
Nulla a magna ac lectus mattis consectetur in porttitor ex. Phasellus vel justo vehicula, posuere dui vitae, placerat mi. Ut non ipsum iaculis, tristique risus et, hendrerit nibh. Vivamus sit amet euismod ipsum. Sed pretium sem at nisi ornare dapibus. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Fusce eget cursus massa. Sed condimentum ante in dui volutpat molestie. Quisque pretium quam a tellus fermentum, ut commodo diam tempus. Phasellus maximus bibendum est eget malesuada.
</p>
<p>
Quisque felis augue, consequat ac varius eget, eleifend eget nunc. Proin et est eget risus ornare sodales rutrum id orci. Aenean tempus, lorem at condimentum congue, diam nulla lacinia ex, ac ultricies metus nisi nec quam. Etiam ac massa id nibh cursus iaculis quis et felis. Morbi nisl risus, blandit sit amet feugiat ut, aliquet at elit. Proin efficitur in mi ac accumsan. Fusce tellus velit, rhoncus vel tempus a, mollis sit amet nunc. In non massa ante.
</p>

      </div></section>
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
