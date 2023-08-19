<template>
  <div id="app">
    <transition :name="transitionName">
      <router-view></router-view>
    </transition>
  </div>
</template>
<script>
export default {
  data() {
    return {
      transitionName: "slide-left",
    };
  },

  watch: {
    $route(to, from) {
      const toDepth = to.meta.depth;
      const fromDepth = from.meta.depth;
      this.transitionName = toDepth < fromDepth ? "slide-right" : "slide-left";
    },
  },
};
</script>
<style lang="scss">
#app {
  font-family: Proxima Nova, Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-color: #f2f2f2;
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

.slide-right-enter-active,
.slide-right-leave-active,
.slide-left-enter-active,
.slide-left-leave-active {
  position: absolute; // 需要注意的地方
  width: 100%; // 需要注意的地方，否则会出现页面渲染卡顿现象
  will-change: transform;
  transition: all 0.3s ease-out;
}

.slide-right-enter {
  
  transform: translate(-100%, 0);
}

.slide-right-leave-active {
  
  transform: translate(0%, 0);
}

.slide-left-enter {
  
  transform: translate(100%, 0);
}

.slide-left-leave-active {
  
  transform: translate(0%, 0);
}
</style>
