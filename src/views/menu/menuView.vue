<template>
  <div class="menu">
    <div class="menu-mask">
      <div class="menu-header">
        <div><img src="./../../assets/Logo.png" alt="" /></div>
        <div>
          <router-link to="/"><i class="el-icon-close"></i></router-link>
        </div>
      </div>
      <div class="menu-content">
        <div class="menu-content__buttom">
          <div class="menu-content__buttom--left">
            <div class="left-1" @click="$router.push({ path: '/about'})">
              <img src="./../../assets/images/menu/Frame-1.png" alt="" />
              <img src="./../../assets/images/menu/Group3.png" alt="" />
            </div>
            <div class="left-2">
              <img src="./../../assets/images/menu/Group86.png" alt="" />
            </div>
          </div>
          <div class="menu-content__buttom--center">
            <div class="left-1">
              <img src="./../../assets/images/menu/Group84.png" alt="" />
            </div>
            <div class="left-2">
              <img src="./../../assets/images/menu/Group85.png" alt="" />
            </div>
          </div>
          <div class="menu-content__buttom--right">
            <div class="left-1">
              <img src="./../../assets/images/menu/Group82.png" alt="" />
            </div>
            <div class="left-2">
              <img src="./../../assets/images/menu/Group83.png" alt="" />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "menuView",
};
</script>
<style lang="scss" scoped>
.menu {
  width: 100%;
  height: 100vh;
  background-image: url("./../../assets/images/bg/29.png");
  background-repeat: no-repeat;
  background-size: cover;
  &-mask {
    width: 100%;
    height: 100vh;
    position: absolute;
    top: 0;
    background: rgb(38, 198, 208);
    background: linear-gradient(
      0deg,
      rgba(38, 198, 208, 0.9) 0%,
      rgba(88, 88, 128, 0.4) 100%
    );
  }
  &-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem 4rem;

    a {
      font-size: 30px;
      color: #ffffff;
    }
  }
  &-content {
    width: 90%;
    margin: 0 auto;
    &__buttom {
      display: flex;
      justify-content: center;
      &--left {
        display: flex;
        flex-direction: column;
        justify-content: center;
        margin-right: 13px;
        .left-1 {
          img {
            cursor: pointer;
            &:nth-child(1) {
              height: 3rem;
              position: absolute;
              margin-left: 30px;
              margin-top: 55px;
            }
            &:nth-child(2) {
              height: 9rem;
            }
          }
        }
        .left-2 {
          img {
            cursor: pointer;
            margin-top: 13px;
            height: 13.5rem;
          }
        }
      }
      &--center {
        .left-1 {
          img {
            cursor: pointer;
            height: 20.5rem;
          }
        }
        .left-2 {
          img {
            cursor: pointer;
            margin-top: 13px;
            height: 13.5rem;
          }
        }
      }
      &--right {
        display: flex;
        flex-direction: column;
        justify-content: center;
        margin-left: 13px;
        .left-1 {
          img {
            cursor: pointer;
            height: 13.5rem;
          }
        }
        .left-2 {
          img {
            cursor: pointer;
            margin-top: 13px;
            height: 9rem;
          }
        }
      }
    }
  }
}
</style>