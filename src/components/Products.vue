<template>
  <div class="bg d-flex justify-around pb-2">
    <ul class="d-flex text">
      <li v-for="(linkimg, index) in linkimgs" :key="index">
        <img :src="linkimage(linkimg)" alt="dc">
        <a :href="linkimg.url">{{ linkimg.text }}</a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "MainProducts",

  data: function () {
    return {
      linkimgs: [
        {
          text: "digital comics",
          img:"buy-comics-digital-comics.png",
          url: "#",
        },

        {
          text: "dc merchandise",
          img:"buy-comics-merchandise.png",
          url: "#",
        },

        {
          text: "subscription",
          img:"buy-comics-subscriptions.png",
          url: "#",
        },

        {
          text: "comic shop locator",
          img:"buy-comics-shop-locator.png",
          url: "#",
        },

        {
          text: "dc power visa",
          img: "buy-dc-power-visa.svg",
          url: "#",
        },
      ],
    };
  },

  methods: {
    linkimage: function(element){
       
     return '../assets/' + 'img/' + element.img;

    }
  }
};
</script>

<style lang = 'scss' scoped>
.bg {
  background-color: rgb(2, 130, 249);
}

.d-flex {
  display: flex;
}

li {
  padding: 20px;
  list-style: none;
  text-transform: uppercase;
  font-weight: bold;
}

a{
  text-decoration: none;
  color: white;
}

.justify-around {
  display: flex;
  justify-content: space-around;
}

.width {
  width: 80px;
  height: 80px;
  padding-top: 20px;
}

.pb-2 {
  padding-bottom: 20px;
}
</style>