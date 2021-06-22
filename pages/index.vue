<template>
  <main>
    <div class = "header-wrapper shadow-lg" >
    <div style="background-color: rgba(0,128,128,1)"
>
    <header class = "container mx-auto pt-4"  >
      <img class = "h-14" src="/img/logoaltreversed.svg" alt="GNOSTIC LOGIC logo" />
 <div class="md:grid grid-cols-2 gap-10 px-10 md:px-0">
           
            <div  class = "py-10">
           <img  src="/img/dev2.svg" style = "display:block;width:100%" alt="GNOSTIC LOGIC" />
            </div>

                  <div  class = "py-10 flex text-center items-center">
                    <div>
            <h1 style = "color:white" class ="font-serif font-bold text-5xl">Modern, innovative {web} development</h1>
                  <button class = "mt-10 py-3 px-9 font-bold  rounded-md w-full md:w-auto" style = "background-color:#F6AE2D">Contact us</button>
                  </div>
                  </div>
      </div>
    </header>
    </div>
        </div>
    <article class="font-sans container mx-auto ">


  <div class="md:grid grid-cols-3 gap-10">
            <div class="p-10 my-10 rounded-none md:rounded-md rounded-none  h-full" style = "background-color:#008080;color:white;">
        <h2 class="font-serif text-4xl font-bold pb-2">Custom solutions</h2>
         <p class = "text-white">
          We believe there isn't a 'one size fits all' approach to web
          development. We won't use
          off-the-shelf templates to design your site: the site will be crafted
          to meet your needs not someone else's.
        </p>
      </div>
                  <div class="p-10 my-10  rounded-none md:rounded-md rounded-none  h-full" style = "background-color:#008080;color:white;">
        <h2 class="font-serif text-4xl font-bold pb-2">Ethical development</h2>
        <p class = "text-white">
        <ul>
          <li>Minimise environmental impact</li>
          <li>Accessible to all</li>
          <li>Respect privacy</li>
        </ul>
        
        </p>
      </div>
                  <div class="p-10 my-10 rounded-none md:rounded-md rounded-none h-full" style = "background-color:#008080;color:white;">
        <h2 class="font-serif text-4xl font-bold pb-2">Cost effective simplicity</h2>
        <p class = "text-white">
        We produce JAMStack websites: static websites powered by powerful serverless APIs. This means smaller bills and less ongoing maintenance.
       
        </p>
      </div>
  </div>
  
    </article> 

  </main>
</template>

<script>
export default {};
</script>

<style lang="scss">
.header-wrapper {
position: relative;
  width: 100%;
  background-image: url('/img/texture2.svg');
}

header .logo-wrapper {
  width: 500px;
  img {
    height: 100%;
    width: 100%;
  }
}
</style>
