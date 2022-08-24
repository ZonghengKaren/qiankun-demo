<template>
  <div id="app">
      <header>
          <router-link to="/">主要用DEMO</router-link> |
          <router-link to="/qiankun-vue1">子应用VUE1</router-link> |
          <router-link to="/qiankun-vue2">子应用VUE2</router-link>
      </header>
      <!-- id为appContainer就是放置子应用的容器 -->
      <div id="appContainer"></div>
      <!-- 用来获取子应用的资源，不做展示 -->
      <div style="display: none" id="microContainer"></div>
      <router-view></router-view>
  </div>
</template>

<script>


export default {
  name: 'App',
  components: {

  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.router-link-exact-active {
    color: red;
}
</style>
