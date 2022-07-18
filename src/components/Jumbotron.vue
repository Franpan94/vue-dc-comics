<template>
  <div class="bg pl-110 pt-50"></div>
</template>

<script>


export default {
  name: "Jumbotron",

  components: {
    Jumbotroncard,
  },
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
</style>