<template>
    <div id="wrapper" class="container-fluid">
        <div class="container" id="main-content">
          <div class="row">
            <div class="col-md-12 col-lg-12 col-xl-12 col-sm-12">
              <Navbar/>
            </div>
          </div>
          <div class="row">
            <div class="col-md-12 col-xl-12 col-lg-12 col-sm-12 divide-line">
              <span>&#10087;</span>
              <span>&#9884;</span>
              <span>&#10087;</span>
            </div>
          </div>
          <div class="row mt-3">
            <router-view/>
          </div>
          <div class="row footer mt-3">
            <div class="col-xl-12 col-md-12 col-lg-12 col-sm-12 p-0">
              <Footer/>
            </div>
          </div>
        </div>
    </div>
</template>

<script lang="ts">
import { Vue, Options } from 'vue-class-component'
import Navbar from '@/components/navbar.vue'
import Footer from '@/components/footer.vue'

@Options({
  components: {
    Navbar,
    Footer
  }
})

export default class Default extends Vue {}
</script>

<style scoped>
#wrapper{
  background: #e0e0e0;
  width: 100%;
}

#main-content{
  background: #f7f7f7;
  overflow: auto;
}

@media only screen and (max-width: 990px) {
  #main-content{
    overflow: visible!important;;
  }
}

.divide-line{
  display: flex;
  justify-content: center;
  font-family: Avenir, Helvetica, Arial, sans-serif;
}

.divide-line span{
  font-size: 30px;
  padding: 5px;
}

.divide-line span:nth-child(1){
  display: inline-block;
  transform: scale(-1, 1);
}
</style>
