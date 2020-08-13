<template>
  <div class="main">
    <h1 class="title">I Cannot Design.</h1>
    <hr>
    <marquee direction="down" width="350" height="200" behavior="alternate">
      <marquee behavior="alternate">
        Under construction!!!1!1one
      </marquee>
    </marquee>
    <img src="/construction.gif"
         height="36"
         width="343"
         alt="This site is under eternal construction.">
    <img src="/underconstruction.gif"
         height="180"
         width="158"
         alt="Still under construction">

    <div>
      <img src="/constjackhammer_e0.gif" alt="An animated construction worker operating a jackhammer.">
      <img src="/anim0206-1_e0.gif"
           alt="A cartoon construction worker eating alternating between eating a sandwich and drinking water.">
      <img src="/constjackhammer_e0.gif" alt="An animated construction worker operating a jackhammer.">
      <img src="/anim0206-1_e0.gif"
           alt="A cartoon construction worker eating alternating between eating a sandwich and drinking water.">
      <img src="/constjackhammer_e0.gif" alt="An animated construction worker operating a jackhammer.">
    </div>

  </div>
</template>

<script>
export default {
  head: {
    meta: [
      { property: 'og:title', content: 'I CANNOT DESIGN' },
      { property: 'og:description', content: 'I THINK i have IT NOW, OOPS, HOLD ON' },
      { property: 'og:type', content: 'website' },
      { property: 'og:url', content: 'https://icannot.design' },
      { property: 'og:image', content: 'https://icannot.design/opengraph.png' },
      { property: 'og:image:height', content: '572' },
      { property: 'og:image:width', content: '1117' },
      { property: 'og:image:alt', content: 'a picture that is a supposed capture of the site, but is off center and cutting off information. Extremely unuseful.' },
    ]
  }
}
</script>

<style>
body {
  background-image: url("/Bglightning.gif");
}

.main {
  min-height: 102vh;
  display: flex;
  flex-flow: column nowrap;
  justify-content: space-around;
  align-items: center;
}

marquee marquee {
  background-color: magenta;
  color: white;
  line-height: 1.2;
  font-family: "Comic Sans", "Comic Sans MS", sans-serif;
}
</style>
