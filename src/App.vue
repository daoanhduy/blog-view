<template>
  <Layout/>
</template>

<script lang="ts">
import { Vue, Options } from 'vue-class-component'
import Layout from '@/layouts/default.vue' // @ is an alias to /src

@Options({
  components: {
    Layout
  }
})

export default class App extends Vue {}
</script>

<style>
*{
  margin: 0;
  padding: 0;
}
body{
  width: 100%;
  height: 100vh;
}
</style>
