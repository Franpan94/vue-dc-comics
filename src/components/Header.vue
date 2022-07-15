<template>
  <div class="d-flex justify-around pb-2">
    <img src="../assets/img/dc-logo.png" alt="dc-logo" class="width" />
    
    <ul class="d-flex text">
      <li v-for="(voice,index) in voices"
      :key="index">{{ voice.text }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "MainHeader",

  data: function(){
    return{
        voices: [
            {
                text: 'characters',
                url: '#'
            },

            {
                text: 'comics',
                url: '#'
            },

            {
                text: 'movies',
                url: '#'
            },

            {
                text: 'tv',
                url: '#'
            },

            {
                text: 'games',
                url: '#'
            },

            {
                text: 'collectibles',
                url: '#'
            },

            {
                text: 'videos',
                url: '#'
            },

            {
                text: 'fans',
                url: '#'
            },

            {
                text: 'news',
                url: '#'
            },

            {
                text: 'shop',
                url: '#'
            },
        ]
    }
},


}
</script>

<style lang = 'scss' scoped>
.bg {
  background-color: rgb(255, 255, 255);
  height: 200px;
}

.d-flex {
  display: flex;
}

li{
    padding: 20px;
    list-style: none;
    cursor: pointer;
    text-transform: uppercase;

    &:hover{
        color: rgb(2, 130, 249);
    }
}

.justify-around{
    display: flex;
    justify-content: space-around;
}

.width{
    width: 80px;
    height: 80px;
    padding-top: 20px;
}

.pb-2{
    padding-bottom: 20px;
}

</style>