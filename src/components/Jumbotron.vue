<template>
  <div class="bg pl-110 pt-50">
    <div class="bg-img justify-end">
        <div class="bg-logo"></div>
    </div>
  </div>
</template>

<script>
export default {
    name: 'MainJumbotron',
}


</script>

<style lang = 'scss' scoped>
.bg {
  background-image: url("../assets/img/jumbotron.jpg");
  height: 100vh;
  background-size: cover;
  background-position: center;
}

.pl-110{
  padding-left: 110px;
}

.pt-50{
  padding-top: 50px;
}

</style>