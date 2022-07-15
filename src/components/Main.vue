<template>
  <section class="bg justify-around">
    <section class="d-flex">
      <ul>
        <h3 class="pt-10">DC COMICS</h3>
        <li v-for="(link, index) in linkone" :key="index">
          <a :href="link.url"></a>{{ link.link }}
        </li>
        <ul class="ml-30">
          <h3 class="pt-10">SHOP</h3>
          <li v-for="(link, index) in linkfour" :key="index">
            <a :href="link.url"></a>{{ link.link }}
          </li>
        </ul>
      </ul>
      <ul>
        <h3 class="pt-10">DC</h3>
        <li v-for="(link, index) in linktwo" :key="index">
          <a :href="link.url"></a>{{ link.link }}
        </li>
      </ul>
      <ul>
        <h3 class="pt-10">SITES</h3>
        <li v-for="(link, index) in linkthree" :key="index">
          <a :href="link.url"></a>{{ link.link }}
        </li>
      </ul>
   </section>
   <div class="bg-logo"></div>
  </section>
</template>

<script>
export default {
  name: "SuperMain",

  data: function () {
    return {
      linkone: [
        {
          link: "digital comics",
          url: "#",
        },

        {
          link: "digital comics",
          url: "#",
        },

        {
          link: "digital comics",
          url: "#",
        },

        {
          link: "digital comics",
          url: "#",
        },

        {
          link: "digital comics",
          url: "#",
        },

        {
          link: "digital comics",
          url: "#",
        },

        {
          link: "digital comics",
          url: "#",
        },
      ],

      linktwo: [
        {
          link: "digital comics",
          url: "#",
        },

        {
          link: "digital comics",
          url: "#",
        },

        {
          link: "digital comics",
          url: "#",
        },

        {
          link: "digital comics",
          url: "#",
        },

        {
          link: "digital comics",
          url: "#",
        },

        {
          link: "digital comics",
          url: "#",
        },

        {
          link: "digital comics",
          url: "#",
        },

        {
          link: "digital comics",
          url: "#",
        },

        {
          link: "digital comics",
          url: "#",
        },
      ],

      linkthree: [
        {
          link: "digital comics",
          url: "#",
        },

        {
          link: "digital comics",
          url: "#",
        },

        {
          link: "digital comics",
          url: "#",
        },

        {
          link: "digital comics",
          url: "#",
        },

        {
          link: "digital comics",
          url: "#",
        },
      ],

      linkfour: [
        {
          link: "digital comics",
          url: "#",
        },

        {
          link: "digital comics",
          url: "#",
        },
      ],
    };
  },
};
</script>

<style lang = 'scss' scoped>
.bg {
  background-image: url("../assets/img/footer-bg.jpg");
  height: 55vh;
  background-size: cover;
  background-position: center;
  color: white;
}

li {
  list-style: none;
  color: grey;
  padding: 3px;
}

.d-flex {
  display: flex;
}

.bg-logo {
  background-image: url("../assets/img/dc-logo-bg.png");
  height: 55vh;
  background-size: cover;
  background-position: center;
  width: 500px;
}

.ml-30 {
  margin-left: -35px;
}

.justify-around{
    display: flex;
    justify-content: space-around;
}
</style>