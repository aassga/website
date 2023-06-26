<template>
  <div>
    <div class="home">
      <div class="home-top__button">
        <div><el-button class="rectangle">START YOUR PROJECT</el-button></div>
        <div>
          <router-link to="/menuView"
            ><img src="./../assets/images/icon/Menu.png" alt=""
          /></router-link>
        </div>
      </div>
      <div class="home-left">
        <div class="home-left__border"></div>
        <div class="home-left__text">DIGITAL AGENCY</div>
      </div>
      <div class="home-title">
        <img src="./../assets/images/bg/Group18.png" alt="" />
        <div class="home-title__content">
          <ul>
            <li>WE CREATE</li>
            <li>AMAZING</li>
            <li>DIGITAL EXPERIENCES</li>
          </ul>
        </div>
      </div>
      <div class="home-bottom">
        <a href="#about"
          ><img src="./../assets/images/icon/Frame.png" alt=""
        /></a>
        <div class="white mb1">TASTE US NOW!</div>
        <div class="home-bottom__border"></div>
      </div>
      <div class="home-iframe">
        <div class="home-iframe__bg"></div>
        <video
          src="./../assets/video/DigiSaladWebsiteVideo-v3.mp4"
          autoplay
          loop="loop"
        ></video>
      </div>
    </div>
    <div class="home-content">
      <aboutPage />
      <div class="home-content__center--buttom">
        <a href="https://www.youtube.com/watch?v=IeIRJ9jZ5Ro" target="_blank">
          <div class="buttom green">
            <div>VIEW MORE</div>
            <div class="border"></div>
          </div>
        </a>
      </div>
      <div class="home-content__rigth">
        <div class="rigth-bg">
          <div class="rigth-bg__left">
            <div class="title">AWARDS</div>
            <img src="./../assets/images/Group61.png" alt="" />
            <div class="content">
              Cras quis nulla commodo, aliquam lectus sed, blandit augue. Cras
              ullamcorper bibendum bibendum. Duis tincidunt urna non pretium
              porta. Nam condimentum vitae ligula vel ornare. Phasellus at
              semper turpis. Nunc eu tellus tortor. Etiam at condimentum nisl,
              vitae sagittis orci. Donec id dignissim nunc.
            </div>
          </div>
          <div class="rigth-bg__right">
            <ul>
              <li v-for="index in 4" :key="index">
                <img src="./../assets/images/image1.png" alt="" />
              </li>
            </ul>
          </div>
        </div>
      </div>
      <div class="home-content__buttom">
        <div class="title">
          <span>OUR INGRADIENTS</span>
          <img src="./../assets/images/Group66.png" alt="" />
        </div>
        <div class="content">
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
        <div class="home-content__center--buttom">
          <div class="buttom purple">
            <div>OUR SERVICES</div>
            <div class="border"></div>
          </div>
        </div>
        <div class="buttom-box">
          <ul>
            <li
              class="buttom-box__li"
              v-for="(item, index) in menuData"
              :key="index"
            >
              <div class="buttom-box__ball">
                <img :src="item.img" alt="" />
              </div>
              <div class="buttom-box__title">{{ item.title }}</div>
              <div class="buttom-box__content">{{ item.content }}</div>
              <div class="buttom-box__buttom">VIEW MORE</div>
            </li>
          </ul>
        </div>
        <div class="content-title">
          <div>VIEW MORE DIGISALAD’S INGRADIENTS</div>
        </div>
      </div>
      <div class="home-content__left">
        <div class="left-bg">
          <div class="left-bg__left">
            <img src="./../assets/images/TST19141.png" alt="" />
            <div class="content">
              <div>Tony Ng</div>
              <div>Founder & Creative Director</div>
            </div>
          </div>
          <div class="left-bg__right">
            <div>
              <img src="./../assets/images/icon/left-quote.png" alt="" />
            </div>
            <div>
              A great digital work isn’t about designing beautiful pages purely.
              It is about context - how do we deliver the <span style="color:yellow">right experience to
              the right person at the right time.</span> The most important thing is
              that your work can engage customers at anytime, anywhere and let
              users experience an entire amazing digital journey.
            </div>
          </div>
        </div>
      </div>
      <div class="home-content__title pt16">
        <span>OUR BRAND EXPERIENCE</span>
        <img src="./../assets/images/Group78.png" alt="" />
      </div>
      <div class="home-content__center">
        <div class="home-content__center--caption flex-direction align-items">
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
          <img class="mt2" src="./../assets/images/DigiSalad.png" alt="" />
        </div>
      </div>
    </div>
    <div class="swiper">
      <swiper :options="swiperOption">
        <swiper-slide v-for="index in 4" :key="index">
          <div class="swiper-box">
            <div class="swiper-num">
              <div class="swiper-num__now">0{{ index }}</div>
              <div class="swiper-num__fan"></div>
              <div class="swiper-num__totle">04</div>
            </div>
            <div class="swiper-box__left">
              <img src="./../assets/images/swiper-img.png" alt="" />
              <div class="swiper-box__left--buttom">
                <div class="buttom green">
                  <div>VIEW PROJECT</div>
                  <div class="border"></div>
                </div>
              </div>
            </div>
            <div class="swiper-box__right">
              <div>HIGHLIGHTED SHOWCASE</div>
              <div>LP CLUB MOBILE APP</div>
              <div>
                Cras quis nulla commodo, aliquam lectus sed, blandit augue. Cras
                ullamcorper bibendum bibendum. Duis tincidunt urna non pretium
                porta. Nam condimentum vitae ligula vel ornare. Phasellus at
                semper turpis. Nunc eu tellus tortor. Etiam at condimentum nisl,
                vitae sagittis orci. Donec id dignissim nunc. Donec elit ante,
                eleifend a dolor et, venenatis facilisis dolor. In feugiat orci
                odio, sed lacinia sem elementum quis. Aliquam consectetur, eros
                et vulputate euismod, nunc leo tempor lacus, ac rhoncus neque
                eros nec lacus. Cras lobortis molestie faucibus.
              </div>
            </div>
          </div>
        </swiper-slide>
        <div class="swiper-button-prev" slot="button-prev"></div>
        <div class="swiper-button-next" slot="button-next"></div>
      </swiper>
    </div>
  </div>
</template>

<script>
import aboutPage from "../components/aboutPage.vue";
import { Swiper, SwiperSlide } from "vue-awesome-swiper";
import "swiper/css/swiper.css";

export default {
  name: "HomeView",
  // 添加组件
  components: {
    Swiper,
    SwiperSlide,
    aboutPage,
  },
  data() {
    return {
      menuData: [
        {
          img: require("./../assets/images/menu/Frame-1.png"),
          title: "UX Design",
          content:
            "Cras quis nulla commodo, aliquam lectus sed, blandit augue. Cras ullamcorper bibendum bibendum. Duis tincidunt urna non pretium porta. Nam condimentum vitae ligula vel ornare.",
        },
        {
          img: require("./../assets/images/menu/Frame-2.png"),
          title: "UI Design",
          content:
            "Cras quis nulla commodo, aliquam lectus sed, blandit augue. Cras ullamcorper bibendum bibendum. Duis tincidunt urna non pretium porta. Nam condimentum vitae ligula vel ornare.",
        },
        {
          img: require("./../assets/images/menu/Frame-3.png"),
          title: "website development",
          content:
            "Cras quis nulla commodo, aliquam lectus sed, blandit augue. Cras ullamcorper bibendum bibendum. Duis tincidunt urna non pretium porta. Nam condimentum vitae ligula vel ornare.",
        },
        {
          img: require("./../assets/images/menu/Frame-4.png"),
          title: "mobile app development",
          content:
            "Cras quis nulla commodo, aliquam lectus sed, blandit augue. Cras ullamcorper bibendum bibendum. Duis tincidunt urna non pretium porta. Nam condimentum vitae ligula vel ornare.",
        },
        {
          img: require("./../assets/images/menu/Frame-5.png"),
          title: "ecommerce",
          content:
            "Cras quis nulla commodo, aliquam lectus sed, blandit augue. Cras ullamcorper bibendum bibendum. Duis tincidunt urna non pretium porta. Nam condimentum vitae ligula vel ornare.",
        },
        {
          img: require("./../assets/images/menu/Frame-6.png"),
          title: "customer loyalty",
          content:
            "Cras quis nulla commodo, aliquam lectus sed, blandit augue. Cras ullamcorper bibendum bibendum. Duis tincidunt urna non pretium porta. Nam condimentum vitae ligula vel ornare.",
        },
        {
          img: require("./../assets/images/menu/Frame-7.png"),
          title: "digital transformation",
          content:
            "Cras quis nulla commodo, aliquam lectus sed, blandit augue. Cras ullamcorper bibendum bibendum. Duis tincidunt urna non pretium porta. Nam condimentum vitae ligula vel ornare.",
        },
        {
          img: require("./../assets/images/menu/Frame-8.png"),
          title: "digital marketing",
          content:
            "Cras quis nulla commodo, aliquam lectus sed, blandit augue. Cras ullamcorper bibendum bibendum. Duis tincidunt urna non pretium porta. Nam condimentum vitae ligula vel ornare.",
        },
        {
          img: require("./../assets/images/menu/Frame-9.png"),
          title: "BRANDING",
          content:
            "Cras quis nulla commodo, aliquam lectus sed, blandit augue. Cras ullamcorper bibendum bibendum. Duis tincidunt urna non pretium porta. Nam condimentum vitae ligula vel ornare.",
        },
      ],
      swiperOption: {
        navigation: {
          prevEl: ".swiper-button-prev", //左侧按钮
          nextEl: ".swiper-button-next", //右侧按钮
        },
        spaceBetween: 1,
        slidesPerView: 1, // 一屏显示的slide个数
        centeredSlides: true, // 居中的slide是否标记为active，默认是最左active,这样样式即可生效
        slideToClickedSlide: true, // 点击的slide会居中
        // loop: true,// 循环播放, 可有无限滚动效果，初始加载即是滚动后的效果
        on: {
          // 该方法中的this都指代swiper本身
          tap: function () {
            console.log("点击的位置", this.activeIndex);
          },
        },
      },
    };
  },
};
</script>
<style lang="scss" scoped>
.swiper {
  width: 100%;
  height: 40rem;
  background-image: url("./../assets/images/LP_fb.png");
  background-size: cover;
  background-position: 0px -36px;
  border-radius: 0 0 30px 30px;
  &-container {
    width: 100%;
    height: 100%;
  }
  &-slide {
    text-align: center;
    font-size: 18px;
  }
  &-button {
    &-prev {
      width: 50px;
      height: 50px;
      border-radius: 50%;
      background-color: #26c4ce;
      left: 55px;
      cursor: pointer;
      &::after {
        font-size: 20px;
        color: #ffffff;
      }
    }
    &-next {
      width: 50px;
      height: 50px;
      border-radius: 50%;
      background-color: #26c4ce;
      right: 55px;
      cursor: pointer;
      &::after {
        font-size: 20px;
        color: #ffffff;
      }
    }
  }
}
.swiper-button-prev.swiper-button-disabled,
.swiper-button-next.swiper-button-disabled {
  opacity: 1;
  pointer-events: auto;
}

.white {
  color: #ffffff;
}
.mb1 {
  margin-bottom: 1rem;
}
.mt2 {
  margin-top: 2rem;
}
.pt16 {
  padding-top: 16rem;
}
.flex-direction {
  flex-direction: column;
}
.align-items {
  align-items: center;
}
.home {
  width: 100%;
  height: 100vh;
  background-image: url("./../assets/images/bg/29.png");
  background-repeat: no-repeat;
  background-size: cover;
  border-radius: 0 0 60px 60px;
  &-iframe {
    width: 100%;
    height: 100vh;
    position: absolute;
    top: 0;
    z-index: 1;
    overflow: hidden;
    &__bg {
      width: 100%;
      height: 100vh;
      position: absolute;
      top: 0;
      background-color: #00000066;
    }
    video {
      width: 1920px;
      height: 1080px;
    }
  }
  &-top {
    &__button {
      z-index: 2;
      display: flex;
      align-items: center;
      justify-content: flex-end;
      position: relative;
      top: 2rem;
      right: 3rem;
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
  &-left {
    z-index: 2;
    height: 100%;
    position: absolute;
    left: -70px;
    display: flex;
    align-items: center;
    color: #ffffff;
    transform: rotate(-90deg);
    &__border {
      width: 9rem;
      height: 0.1rem;
      background-color: #ffffff;
      border-radius: 10px;
    }
    &__text {
      padding-left: 15px;
    }
  }
  &-title {
    z-index: 2;
    margin-left: 25rem;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    position: absolute;
    top: 35%;
    img {
      height: 3.5rem;
    }
    &__content {
      margin-top: 1rem;
      text-align: left;
      ul {
        line-height: 1rem;
        line-height: 4rem;
        li {
          font-size: 38px;
          color: #ffffff;
          font-weight: 600;
        }
      }
    }
  }
  &-bottom {
    z-index: 2;
    width: 100%;
    text-align: center;
    position: absolute;
    bottom: 80px;
    img {
      cursor: pointer;
    }
    &__border {
      width: 0.1rem;
      height: 10rem;
      position: absolute;
      left: 50%;
      background: rgb(255, 255, 255);
      background: linear-gradient(
        180deg,
        rgba(255, 255, 255, 1) 0%,
        rgba(255, 255, 255, 1) 50%,
        rgba(0, 0, 0, 1) 50%,
        rgba(0, 0, 0, 1) 100%
      );
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

    &__rigth {
      width: 100%;
      margin-top: 5rem;
      display: flex;
      justify-content: flex-end;
      position: absolute;
      .rigth-bg {
        width: 88%;
        height: auto;
        background-color: #ffffff;
        padding: 4rem;
        border-radius: 30px 0px 30px 30px;
        display: flex;
        align-items: center;
        &__left {
          width: 23rem;
          padding-right: 12rem;
          margin-left: 12rem;
          .title {
            font-size: 28px;
            font-weight: 600;
          }
          img {
            width: 10rem;
          }
          .content {
            text-align: left;
            line-height: 1.5rem;
            margin-top: 2rem;
          }
        }
        &__right {
          width: 46rem;
          ul {
            display: flex;
            flex-wrap: wrap;
            li {
              margin-right: 20px;
              margin-bottom: 20px;
            }
          }
        }
      }
    }
    &__buttom {
      width: 100%;
      background-color: #26c6d0;
      border-radius: 30px;
      margin-top: 15rem;
      .title {
        padding-top: 20rem;
        font-size: 34px;
        font-weight: 600;
        display: flex;
        flex-direction: column;
        align-items: center;
        color: #ffffff;
      }
      .content {
        display: flex;
        justify-content: center;
        margin: 45px 0;
        div {
          width: 56rem;
          line-height: 1.5rem;
          color: #ffffff;
        }
      }
    }
    &__left {
      width: 100%;
      margin-top: -15rem;
      display: flex;
      justify-content: flex-start;
      position: absolute;
      .left-bg {
        width: 88%;
        height: auto;
        background-image: url("./../assets/images/bg/shutterstock.png");
        background-size: cover;
        padding: 4rem;
        border-radius: 0px 30px 30px 30px;
        display: flex;
        align-items: center;
        &__left {
          width: 23rem;
          padding-right: 12rem;
          margin-left: 12rem;
          img {
            width: 10rem;
            border-radius: 50%;
          }
          .content {
            line-height: 1.5rem;
            margin-top: 2rem;
            color: #fff;
            div {
              &:nth-child(1) {
                text-transform: uppercase;
                font-weight: 600;
              }
              &:nth-child(2) {
                font-style: oblique;
              }
            }
          }
        }
        &__right {
          div {
            &:nth-child(2) {
              width: 33rem;
              text-align: left;
              line-height: 2rem;
              color: #fff;
              letter-spacing: 2px;
            }
          }
        }
      }
    }
  }
}
.green {
  background-color: #26c6d0;
}
.purple {
  background-color: #585880;
}

.home-content__center--buttom,
.swiper-box__left--buttom {
  width: 100%;
  display: flex;
  justify-content: center;
  cursor: pointer;
  a {
    text-decoration: none;
  }
  .buttom {
    padding: 23px;
    display: flex;
    align-items: center;
    color: #ffffff;
    font-weight: 600;

    .border {
      width: 66px;
      height: 0.1rem;
      margin-left: 15px;
      background-color: #ffffff;
    }
  }
}
.swiper-box__left--buttom {
  width: 100%;
  display: flex;
  justify-content: center;
  cursor: pointer;
  z-index: 9;
  margin-top: 27rem;
  .buttom {
    padding: 4rem;
  }
}
.buttom {
  &-box {
    display: flex;
    justify-content: space-around;
    margin-top: 5rem;
    ul {
      display: flex;
      width: 75rem;
      flex-wrap: wrap;
    }
    &__li {
      display: flex;
      flex-direction: column;
      width: 15rem;
      align-items: center;
      padding: 5rem;
      color: #ffffff;
    }
    &__ball {
      width: 5rem;
      height: 5rem;
      border-radius: 50%;
      background-color: #ffffff;
      display: flex;
      align-items: center;
      justify-content: center;
      img {
        width: 2rem;
      }
    }
    &__title {
      height: 75px;
      line-height: 25px;
      font-size: 20px;
      width: 10rem;
      display: flex;
      align-items: center;
      text-transform: uppercase;
      font-weight: 600;
      justify-content: center;
    }
    &__content {
      font-size: 16px;
      width: 19rem;
      line-height: 1.3rem;
    }
    &__buttom {
      border: 1px solid #ffffff;
      padding: 1.3rem 3rem;
      border-radius: 40px;
      margin-top: 2rem;
      cursor: pointer;
    }
  }
}
.content {
  &-title {
    font-size: 18px;
    color: #ffffff;
    font-weight: 600;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding-bottom: 20rem;
    div {
      &:nth-child(1) {
        z-index: 9;
      }
    }
    &::after {
      content: "";
      display: block;
      width: 22rem;
      height: 0.3rem;
      background-color: #ffbc58;
      position: absolute;
      margin-top: 10px;
    }
  }
}
.swiper {
  &-num {
    color: #fff;
    width: 4rem;
    position: absolute;
    right: 8rem;
    top: 5rem;
    &__now {
      text-align: left;
    }
    &__fan {
      width: 4rem;
      height: 0.1rem;
      background: #26c6d0;
      transform: rotate(148deg);
    }
    &__totle {
      text-align: right;
    }
  }
  &-box {
    height: 100%;
    display: flex;
    &__left {
      width: 50%;
      height: 100%;
      display: flex;
      align-items: center;
      img {
        height: 25rem;
        position: relative;
        left: 15rem;
      }
    }
    &__right {
      color: #ffffff;
      width: 32%;
      display: flex;
      align-items: flex-start;
      flex-direction: column;
      justify-content: center;
      text-align: left;
      line-height: 1.5rem;

      div {
        &:nth-child(1) {
          font-size: 16px;
        }
        &:nth-child(2) {
          z-index: 9;
          font-size: 32px;
          height: 5rem;
          line-height: 5rem;

          &::after {
            content: "";
            display: block;
            width: 20.5rem;
            height: 0.3rem;
            background-color: #26c6d0;
            position: absolute;
            margin-top: -33px;
            z-index: -1;
          }
        }
        &:nth-child(3) {
          font-size: 16px;
        }
      }
    }
  }
}
</style>