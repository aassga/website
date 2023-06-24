<template>
  <div class="about">
    <div class="about-header">
      <div><img src="./../assets/Logo.png" alt="" /></div>
      <div class="about-top__button">
        <div><el-button class="rectangle">START YOUR PROJECT</el-button></div>
        <div>
          <router-link to="/menuView"
            ><img src="./../assets/images/icon/Menu.png" alt=""
          /></router-link>
        </div>
      </div>
    </div>
    <div class="about-content">
      <div class="about-content__title">
        <span>ABOUT DIGISALAD</span>
        <img src="./../assets/images/Group61.png" alt="" />
      </div>
      <div class="about-content__center">
        <img src="./../assets/images/Group60.png" alt="" />
        <div class="about-content__center--caption">
          <div>
            Cras quis nulla commodo, aliquam lectus sed, blandit augue. Cras
            ullamcorper bibendum bibendum. Duis tincidunt urna non pretium
            porta. Nam condimentum vitae ligula vel ornare. Phasellus at semper
            turpis. Nunc eu tellus tortor. Etiam at condimentum nisl, vitae
            sagittis orci. Donec id dignissim nunc. Donec elit ante, eleifend a
            dolor et, venenatis facilisis dolor. In feugiat orci odio, sed
            lacinia sem elementum quis. Aliquam consectetur, eros et vulputate
            euismod, nunc leo tempor lacus, ac rhoncus neque eros nec lacus.
            Cras lobortis molestie faucibus.
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<style lang="scss" scoped>
.about {
  // width: 100%;
  // height: 100vh;
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
    &__center {
      margin-top: 5rem;
      width: 100%;

      &--caption {
        display: flex;
        justify-content: center;

        padding: 45px 0;
        div {
          width: 56rem;
          line-height: 1.5rem;
        }
      }
    }
  }
}
</style>