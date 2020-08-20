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
    };
  },
  computed:{
    myRoute(){
      const hash = this.$route.hash.slice(1) || 'index';
      return `svg-pages/${hash}.svg#default`;
    },
    myViewBox(){
      return `0 0 ${this.width} ${this.height}`;
    }
  },
  mounted(){
    if(process.client){
      this.height = window.innerHeight;
      this.width = window.innerWidth;
      window.addEventListener('resize', ()=>{
        this.height = window.innerHeight;
        this.width = window.innerWidth;
      })
    }

  }
}
</script>

<style scoped>

</style>
