<template>
    <footer class="footer-page">
        <p class="m-0 pt-2 pb-2">Copyright by Đào Anh Duy <sup>&#169;</sup> 2022</p>
    </footer>
</template>

<script>
import { Vue } from 'vue-class-component'

export default class Footer extends Vue {}
</script>

<style scoped>
p{
    font-family: 'Lora', serif;
    text-align: center;
    letter-spacing: 1px;
    color: #fff;
}
.footer-page{
    background: #000;
}
</style>
