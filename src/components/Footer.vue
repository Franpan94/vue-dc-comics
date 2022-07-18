<template>
    <div class="bg d-flex-around">
        <button class="utilities cursor">SIGN-UP NOW!</button>
        <div class="d-flex">
            <h3 class="color p-10">FOLLOW US</h3>
           <div class="p-10" v-for="(img,index) in imgs"
             :key="index">
                <img :src="require(`../assets/img/${img.img}`)" alt="dc" class="cursor">
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
                    img: 'footer-twitter.png',
                    url: '#',
                },

                {
                    img: 'footer-youtube.png',
                    url: '#',
                },

                {
                    img: 'footer-pinterest.png',
                    url: '#',
                },

                {
                    img: 'footer-periscope.png',
                    url: '#',
                },
            ],
        };
    },
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

.cursor{
    cursor: pointer;
}

.color{
    color: rgb(2, 130, 249);
}

.p-10{
    padding: 10px;
}

</style>