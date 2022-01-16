<template>
    <div class="col-md-8 col-xl-8 col-lg-8 col-sm-8">
        <BlogItem/>
    </div>
    <div class="col-md-4 col-xl-4 col-lg-4 col-sm-4">
        <div class="row" style="position: relative">
            <span class="title-category">Danh Mục</span>
            <div class="col-md-12 col-xl-12 col-lg-12 col-sm-12 list-categories">
                <ul>
                    <li v-for="i in 5" :key="i">
                        {{i}}
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script lang="ts">
import { Vue, Options } from 'vue-class-component'
import BlogItem from '@/components/blog_item.vue'
import { HOME_TITLE } from '@/utils/constant'

@Options({
  components: {
    BlogItem
  }
})

export default class Home extends Vue {
    beforeCreate(){
        document.title = HOME_TITLE
    }
}
</script>

<style scoped>
.list-categories ul{
    list-style: '\27A3';
    padding-left: 15px;
}
.title-category{
    font-family: 'Lora', serif;
    font-weight: bold;
}
.title-category::before{
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    background: #000;
    width: 5px;
    margin-top: 3px;
    height: 20px;
}
.list-categories{
    font-family: 'Lora', serif;
    padding: 0;
}
.list-categories ul li{
    padding-left: 15px;
    padding-bottom: 10px;
    margin-top: 10px;
    margin-bottom: 10px;
    border-bottom: 1px solid #dedede;
}
</style>
