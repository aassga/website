<template>
  <div id="app">
    <router-view v-slot="{ Component, route }">
      <!-- 使用任何自定义过渡和回退到 `fade` -->
      <transition :name="route.meta.transition || 'fade'">
        <component :is="Component" />
      </transition>
    </router-view>
  </div>
</template>

<style lang="scss">
#app {
  font-family: Proxima Nova, Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
