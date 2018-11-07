<template>
  <div>
    <div class="header">
      <v-header></v-header>
    </div>
    <div class="tab">
      <div class="tab-item">
        <router-link to="/goods">商品</router-link>
      </div>
      <div class="tab-item">
        <router-link to="/ratings">评论</router-link>
      </div>

      <div class="tab-item">
        <router-link to="/seller">商家</router-link>
      </div>
    </div>
    <router-view></router-view>
  </div>
</template>

<script>
  import header from './components/header/header.vue'

  export default {
    components: {
      'v-header': header
    }
  }
</script>

<style>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }

  .tab {
    display: flex;
    width: 100%;
    height: 40px;
    line-height: 40px;
  }

  .tab-item {
    flex: 1;
    text-align: center;
  }
</style>
