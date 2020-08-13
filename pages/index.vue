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
      { property: 'og:image:alt', content: 'a picture that is a supposed capture of the site, but is off center and cutting off information. Extremely unuseful.' },
      { name:'twitter:card', content:'summary_large_image'},
      { name:'twitter:site', content:'icannot.design?'},
      { name:'twitter:creator', content:'fimion'},
      { name:'twitter:title', content:'I CANNOT DESIGN'},
      { name:'twitter:description', content:'I THINK i have IT NOW, OOPS, HOLD ON'},
      { name:'twitter:image', content: 'https://icannot.design/opengraph.png' },
      { name:'twitter:image:alt', content: 'a picture that is a supposed capture of the site, but is off center and cutting off information. Extremely unuseful.' },
    ],
    link: [
      { rel: 'stylesheet', href: 'https://fonts.googleapis.com/css2?family=Lacquer&display=swap'},
    ]
  }
}
</script>

<style>
h1, h2, h3, h4, h5, h6 {
  font-family: 'Lacquer', cursive;
  font-weight: 400;
  color: magenta;
  text-shadow: 0 0 10px turquoise;
}

hr{
  width: 546px;
  border: none;
  border-top: 30px solid;
  border-image-source: url("/anismilebar.gif");
  background: url("/anismilebar.gif") center top;
}
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

a.github-link{
  left:0;
  right: unset;
}
.octo-arm,.octo-body{
  fill:teal;
}
.octo-bg{
  fill:hotpink;
  stroke: teal;
  stroke-width: 10;
}
</style>
