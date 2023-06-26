<template>
  <div id="about">
    <div class="about-content__title">
      <span>ABOUT DIGISALAD</span>
      <img src="./../assets/images/Group61.png" alt="" />
    </div>
    <div class="about-content__center">
      <a href="https://www.youtube.com/watch?v=IeIRJ9jZ5Ro" target="_blank"><img src="./../assets/images/Group60.png" alt="" /></a>
      <div class="about-content__center--caption">
        <div>
          Cras quis nulla commodo, aliquam lectus sed, blandit augue. Cras
          ullamcorper bibendum bibendum. Duis tincidunt urna non pretium porta.
          Nam condimentum vitae ligula vel ornare. Phasellus at semper turpis.
          Nunc eu tellus tortor. Etiam at condimentum nisl, vitae sagittis orci.
          Donec id dignissim nunc. Donec elit ante, eleifend a dolor et,
          venenatis facilisis dolor. In feugiat orci odio, sed lacinia sem
          elementum quis. Aliquam consectetur, eros et vulputate euismod, nunc
          leo tempor lacus, ac rhoncus neque eros nec lacus. Cras lobortis
          molestie faucibus.
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "aboutPage",

};
</script>
<style scoped lang="scss">
.about {
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
