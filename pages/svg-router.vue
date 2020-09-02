<template>
  <div class="main">
    <svg :viewBox="myViewBox">
      <use :href="myRoute" />
    </svg>
  </div>
</template>

<script>
export default {
  name: 'svg-router',
  layout: 'handrawn',
  head:{
    meta:[
      { property: 'og:url', content: 'https://icannot.design/svg-router/' },
      { property: 'og:image', content: 'https://icannot.design/page-previews/svg-router.jpg' },
      { property: 'og:image:alt', content: 'a picture that is a supposed capture of the site, but is off center and cutting off information. Extremely unuseful.' },
      { name:'twitter:image', content: 'https://icannot.design/page-previews/svg-router.jpg' },
      { name:'twitter:image:alt', content: 'a picture that is a supposed capture of the site, but is off center and cutting off information. Extremely unuseful.' },
    ],
  },
  data(){
    return {
      height: 100,
      width: 100,
      hash: 'index',
    };
  },
  computed:{
    myRoute(){
      const hash = this.hash;
      return `/svg-pages/${hash}.svg#default`;
    },
    myViewBox(){
      const height = this.height;
      const width = this.width;
      return `0 0 ${width} ${height}`;
    }
  },
  methods:{
    setHashValue(route){
      this.$nextTick(()=>{
        this.hash = route.hash.slice(1) || 'index';
      })
    },
    setWindowSize(){
      this.height = window.innerHeight;
      this.width = window.innerWidth;
    }
  },
  mounted(){
    if(process.client){
      this.setWindowSize();
      window.addEventListener('resize', this.setWindowSize);
      this.setHashValue(this.$route);
    }
  },
  watch:{
    '$route':{
      deep: true,
      immediate: true,
      handler(newVal, oldVal){
        console.log(newVal, oldVal);
        const oldHash = oldVal ? oldVal.hash : '';
        if(newVal && (newVal.hash !== oldHash)){
          this.setHashValue(newVal);
        }
      }
    }
  },
}
</script>

<style scoped>

</style>
