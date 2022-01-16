<template>
    <nav class="navbar navbar-expand-lg">
        <div class="container-fluid menu-main">
            <router-link class="navbar-brand" to="/">Anh Duy IT</router-link>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <ul class="navbar-nav">
                    <li class="nav-item">
                        <!-- <router-link to="/">Home</router-link> -->
                        <router-link class="nav-link" to="/">Trang chủ</router-link>
                    </li>
                    <li class="nav-item">
                        <router-link class="nav-link" to="/">Giới thiệu</router-link>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
</template>

<script lang="ts">
import { Vue } from "vue-class-component";

export default class Navbar extends Vue {}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Dancing+Script:wght@400;500;600&family=Varela+Round&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Lora&display=swap');
.menu-main{
    padding-left: 5px;
    padding-right: 5px;
}
.navbar-brand{
    font-family: 'Dancing Script', cursive;
    font-size: 40px;
    color: #000;
    transition: .5s;
}

.navbar-brand:hover{
    color: #b6b6b6;
}

#navbarSupportedContent{
    justify-content: flex-end;
    align-items: center;
}

.nav-item a{
    font-family: 'Lora', serif;
    color: #000;
    transition: .5s;
    letter-spacing: 2px;
    text-align: center;
}

.nav-item a:hover{
    color: #b6b6b6;
}

@media only screen and (max-width: 990px)  {
    .navbar-brand{
        font-size: 25px!important;
    }
}
</style>