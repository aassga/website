<template>
  <div class="menu">
    <div class="menu-header">
      <div><img src="./../../assets/Logo.png" alt=""></div>
      <div>
        <router-link to="/"
          ><i class="el-icon-close"></i></router-link>
      </div>
    </div>
    <div class="menu-content"></div>
  </div>
</template>

<script>


export default {
  name: 'menuView',

}
</script>
<style lang="scss" scoped>
  .menu{
    width: 100%;
    height: 100vh;
    background-image: url("./../../assets/images/bg/29.png");
    background-repeat: no-repeat;
    background-size: cover;
    &-header{
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 1rem 4rem;
      background: #FFFFFF
      a{
        font-size: 30px;
        color: #FFFFFF;
      }
    }
  }
</style>