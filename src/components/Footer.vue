<template>
    <div class="bg d-flex-around">
        <button class="utilities">SIGN-UP NOW!</button>
        <div class="d-flex">
            <h3 class="color p-10">FOLLOW US</h3>
           <div class="p-10" v-for="(img,index) in imgs"
             :key="index">
                <img :src="linkimage(img)" alt="dc">
           </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'MainFooter',
    data: function(){
        return{
            imgs:[
                {
                    img: 'footer-facebook.png',
                    url: '#',
                },

                {
                    img: 'footer-facebook.png',
                    url: '#',
                },

                {
                    img: 'footer-facebook.png',
                    url: '#',
                },

                {
                    img: 'footer-facebook.png',
                    url: '#',
                },

                {
                    img: 'footer-facebook.png',
                    url: '#',
                },
            ],
        };
    },

    methods: {
    linkimage: function(element){
       
     return '../assets/' + 'img/' + element.img;

    }
  }
}


</script>

<style lang = 'scss' scoped>

.bg{
   background-color: rgb(48, 48, 48);
   height: 100px;
}

.d-flex-around{
    display: flex;
    justify-content: space-around;
    align-items: center;
}

.d-flex{
    display: flex;
    align-items: center;
}

.utilities{
    padding: 10px;
    border: 4px solid rgb(2, 130, 249);
    background-color:rgb(48, 48, 48) ;
    color: white;
}

.color{
    color: rgb(2, 130, 249);
}

.p-10{
    padding: 10px;
}

</style>