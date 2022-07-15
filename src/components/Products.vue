<template>
  <div class="d-flex justify-around pb-2">
    <img src="../assets/img/dc-logo.png" alt="dc-logo" class="width" />

    <ul class="d-flex text">
      <li v-for="(voice, index) in voices" :key="index"><a :href="voice.url">{{ voice.text }}</a> </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "MainHeader",

  data: function () {
    return {
      voices: [
        {
          text: "characters",
          url: "#",
        },

        {
          text: "comics",
          url: "#",
        },

        {
          text: "movies",
          url: "#",
        },

        {
          text: "tv",
          url: "#",
        },

        {
          text: "games",
          url: "#",
        },

        {
          text: "collectibles",
          url: "#",
        },

        {
          text: "videos",
          url: "#",
        },

        {
          text: "fans",
          url: "#",
        },

        {
          text: "news",
          url: "#",
        },

        {
          text: "shop",
          url: "#",
        },
      ],
    };
  },
};
</script>

<style>
.bg{
    background-color: rgb(2, 130, 249);
    
}
</style>