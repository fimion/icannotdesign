<script>
import DefaultLayout from './default.vue';
export default {
  name: 'purple',
  extends: DefaultLayout,
  head:{
    link: [
      { rel: 'stylesheet', href: 'https://fonts.googleapis.com/css2?family=Lacquer&display=swap'},
    ]
  },
}
</script>
<style scoped>
* >>>h1.title{
  text-align: center;
}

  * >>> h1, * >>> h2, * >>> h3, * >>> h4, * >>> h5, * >>> h6 {
    font-family: 'Lacquer', cursive;
    font-weight: 400;
    color: magenta;
    text-shadow: 0 0 10px turquoise;
  }

  * >>> h1 a, * >>> h1 a:hover, * >>> h1 a:focus, * >>> h1 a:visited,
  * >>> h2 a, * >>> h2 a:hover, * >>> h2 a:focus, * >>> h2 a:visited,
  * >>> h3 a, * >>> h3 a:hover, * >>> h3 a:focus, * >>> h3 a:visited,
  * >>> h4 a, * >>> h4 a:hover, * >>> h4 a:focus, * >>> h4 a:visited,
  * >>> h5 a, * >>> h5 a:hover, * >>> h5 a:focus, * >>> h5 a:visited,
  * >>> h6 a, * >>> h6 a:hover, * >>> h6 a:focus, * >>> h6 a:visited
  {
    color: inherit;
  }

  * >>> a, * >>> a:hover, * >>> a:focus, * >>> a:visited {
    color: forestgreen;
    text-shadow: 0 0 5px darkorchid;
  }


* >>> hr {
    width: 546px;
    border: none;
    border-top: 30px solid;
    border-image-source: url("/anismilebar.gif");
    background: url("/anismilebar.gif") center top;
  }

  .layout {
    background-image: url("/Bglightning.gif");
    min-height: 100vh;
    min-width: 100vw;
    padding: 20px;
  }

  .main {
    min-height: 102vh;
    display: flex;
    flex-flow: column nowrap;
    justify-content: space-around;
    align-items: center;
  }

  * >>> a.github-link {
    left: 0;
    right: unset;
  }

  * >>> .octo-arm, * >>> .octo-body {
    fill: teal;
  }

  * >>> .octo-bg {
    fill: hotpink;
    stroke: teal;
    stroke-width: 10;
  }
</style>

