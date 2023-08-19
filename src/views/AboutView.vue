<template>
  <div class="about">
    <div class="about-header">
      <div @click="$router.push({path:'/'})"><img src="./../assets/Logo-1.png" alt="" /></div>
      <div class="about-top__button">
        <div><el-button class="rectangle" @click="$router.push({path:'/'})">START YOUR PROJECT</el-button></div>
        <div>
          <router-link to="/menuView"
            ><img src="./../assets/images/icon/Menu-simple-line-icons.png" alt=""
          /></router-link>
        </div>
      </div>
    </div>
    <div class="about-content">
     <aboutPage />
    </div>
  </div>
</template>
<script>
import aboutPage from "../components/aboutPage.vue";
export default {
  components: {
    aboutPage,
  },
}
</script>
<style lang="scss" scoped>
.about {
  &-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem 4rem;
    background: #FFFFFF
    a {
      font-size: 30px;
      color: #ffffff;
    }
    img{
      cursor: pointer;
    }
  }
  &-top {
    &__button {
      display: flex;
      align-items: center;
      justify-content: flex-end;
      position: relative;
      top: 3px;
      right: 1px;
      div {
        &:nth-child(1) {
          margin-right: 2.5rem;
        }
        &:nth-child(2) {
          cursor: pointer;
        }
      }
      .rectangle {
        background: rgb(78, 229, 234);
        background: linear-gradient(
          207deg,
          rgba(78, 229, 234, 1) 100%,
          rgba(38, 208, 168, 1) 100%
        );
        color: #ffffff;
        font-weight: 600;
        border-radius: 30px;
      }
    }
  }
  &-content {
    margin-top: 7rem;
    &__title {
      font-size: 34px;
      font-weight: 600;
      display: flex;
      flex-direction: column;
      align-items: center;
    }
  }
}
</style>