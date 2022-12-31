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
    },
    onHashChange(e){
      this.setHashValue(window.location)
    }
  },
  mounted(){
    this.setWindowSize();
    window.addEventListener('resize', this.setWindowSize);
    this.setHashValue(window.location);
    window.addEventListener('hashchange',this.onHashChange);
  },
  beforeUnmount() {
    window.removeEventListener('hashchange',this.onHashChange);
  }
}
</script>

<style scoped>

</style>
