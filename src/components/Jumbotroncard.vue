<template>
   <div class="width">
       <img :src="thumburl" :alt="serie" class="widthimg">
       <h4>{{ serie }}</h4>
   </div>
</template>

<script>
export default {
    props: {
        'thumburl': String,
        'currentprice': String,
        'serie': String,
        'currentype': String,
    }
}
</script>

<style lang = 'scss' scoped>
  .width{
   color: white;
   width: calc(100% / 6);
   margin: auto;
  }

   .widthimg{
     height: 200px;
   }

   
</style>