<template>
  <main>
    <header>
      <div class="flex header-wrapper justify-center pb-48 pt-10">
        <div class="logo-wrapper">
          <img src="/img/logoalt.svg" alt="GNOSTIC LOGIC" />
        </div>
      </div>

    </header>
    <article class="font-sans container mx-auto" style = "margin-top:-50px;">



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
  background-image: url('/img/texture.svg');
}
.header-wrapper::after{
    position: absolute;
    bottom:0px;
    left:0px;
    right:0px;
    top:0px;
    background-size: cover;
    background-image: linear-gradient(
    to bottom,
    rgba(231, 238, 237, 0),
    rgba(231, 238, 237, 1)
  );
}

header .logo-wrapper {
  width: 500px;
  img {
    height: 100%;
    width: 100%;
  }
}
</style>
