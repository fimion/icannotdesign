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

