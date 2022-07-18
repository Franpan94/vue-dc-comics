<template>
  <div class="bg pl-110 pt-50 position-relative">
    <div class="bg-series position-absolute">Current series</div>
  </div>
</template>

<script>


export default {
  name: "Jumbotron",
};
</script>

<style lang = 'scss' scoped>
.bg {
  background-image: url("../assets/img/jumbotron.jpg");
  height: 40vh;
  background-size: cover;
}

.pl-110 {
  padding-left: 110px;
}

.pt-50 {
  padding-top: 50px;
}

.bg-series{
  background-color: rgb(2, 130, 249);
  display: inline-block;
  padding: 10px;
  text-transform: uppercase;
  font-weight: bold;
  color: white;
}

.position-relative{
  position: relative;
}

.position-absolute{
  position: absolute;
  bottom: -20px;
  left: 6rem;
  z-index: 1;
}
</style>