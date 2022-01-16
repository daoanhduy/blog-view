<template>
    <div class="blog-item" v-for="i in 15" :key="i">
        <img src="../static/images/image_1.jpeg" alt="">
        <div class="content-item">
            <router-link to='/blog/detail/1' class="content-item-title"><h4>Đằng sau cái kết của ‘No Time to Die’</h4></router-link>
            <p>Đạo diễn Cary Joji Fukunaga tiết lộ cái kết của “No Time to Die” đã được ngầm thông báo với khán giả ngay từ nửa đầu bộ phim.
                <router-link to="/" class="read-more">Xem thêm</router-link>
            </p>
            <div class="blog-info mt-auto">
                <span>26-1-2022</span>
                <span>Anh Duy</span>
            </div>
        </div>
    </div>
</template>

<script lang="ts">
import { Vue } from 'vue-class-component'

export default class BlogItem extends Vue {

}
</script>

<style scoped>
.blog-item{
    position: relative;
    display: flex;
    width: 100%;
    margin-bottom: 50px;
}

@media only screen and (max-width: 990px)  {
    .blog-item{
        flex-direction: column;
    }

    .blog-item img{
        width: 100%!important;
    }

    .content-item{
        width: 100%!important;
        padding: 5px 0 0 0!important;
    }
}

.blog-item img{
    width: 40%;
    height: 250px;
}

.content-item-title{
    font-family: 'Dancing Script', cursive;
    
    text-decoration: none;
    color: #000;
}

.content-item-title h4{
    font-size: 25px;
    font-weight: bold;
}

.content-item{
    width: 55%;
    padding: 0 15px 0 15px;
    letter-spacing: 1.2px;
    display: flex;
    flex-direction: column;
}

.content-item p {
    font-family: 'Lora', serif;
}

.read-more{
    text-decoration: none;
}
.blog-info{
    display: flex;
    padding-top: 20px;
    justify-content: space-between;
    align-items: flex-end;
}
.blog-info span{
    font-family: 'Dancing Script', cursive;
    font-size: 15px;
    font-style: italic;
    font-weight: bold;
}
</style>
