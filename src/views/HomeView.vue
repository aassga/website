<template>
  <div class="home">
    <div class="home-top__button"> 
      <div><el-button class="rectangle">START YOUR PROJECT</el-button></div>
      <div><router-link to=""><img src="./../assets/images/icon/Menu.png" alt=""></router-link></div>
    </div>
    <div class="home-left">
      <div class="home-left__border"></div>
      <div class="home-left__text">DIGITAL AGENCY</div>
    </div>
    <div class="home-title">
      <img src="./../assets/images/bg/Group18.png" alt="">
      <div class="home-title__content">
        <ul>
          <li>WE CREATE</li>
          <li>AMAZING </li>
          <li>DIGITAL EXPERIENCES</li>
        </ul>
      </div>
      
    </div>
  </div>
</template>

<script>


export default {
  name: 'HomeView',

}
</script>
<style lang="scss" scoped>
  .home{
    width: 100%;
    height: 100vh;
    background-image: url(http://localhost:8080/img/29.b7185c65.png);
    background-repeat: no-repeat;
    background-size: cover;
    &-top{
      &__button{
        display: flex;
        align-items: center;
        justify-content: flex-end;
        position: relative;
        top: 2rem;
        right: 3rem;
        div{
          &:nth-child(1){
            margin-right: 2.5rem;
          }
          &:nth-child(2){
            cursor: pointer;
          }
        }
        .rectangle{
          background: rgb(78,229,234);
          background: linear-gradient(207deg, rgba(78,229,234,1) 100%, rgba(38,208,168,1) 100%);
          color: #FFFFFF;
          font-weight: 600;
          border-radius: 30px;
        }
      }
    }
    &-left{
      height: 100%;
      position: absolute;
      left: -70px;
      display: flex;
      align-items: center;
      color: #FFFFFF;
      transform: rotate(-90deg);
      &__border{
        width: 9rem;
        height: 0.1rem;
        background-color: #FFFFFF;
        border-radius: 10px;
      }
      &__text{
        padding-left: 15px;
      }
    }
    &-title{    
      height: 100%;
      margin-left: 25rem;
      display: flex;
      flex-direction: column;
      align-content: flex-start;
      justify-content: center;
      align-items: flex-start;
      img{
        height: 3.5rem;
      }
      &__content{
        margin-top: 1rem;
        text-align: left;
        ul{
          line-height: 1rem;
          line-height: 4rem;
          li{
            font-size: 38px;
            color: #FFFFFF;
            font-weight: 600;
          }
        }
      }
    }
  }
</style>