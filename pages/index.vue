<template>
  <div class="main">
    <h1 class="title">I Cannot Design.</h1>
    <hr>
    <img src="/construction.gif"
         height="36"
         width="343"
         alt="This site is under eternal construction.">

  </div>
</template>

<script>
export default {}
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
.title{
  color: white;
}
</style>
