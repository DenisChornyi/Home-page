<template>


  <hooper :infiniteScrol="true" :autoPlay="true" :transition="600" :playSpeed="3500" :wheelControl="false">
    <slide class="slide1">
      <div class="container">
        <div class="slide-title">
            <h4 class="slide-title-h4 wow slideInUp delay-2s">A range of programs for women's healthcare</h4>
            <h1 class="slide-title-h1 wow slideInUp delay-2s">Special Touch</h1>
            <button class="slide-title-button button wow slideInUp delay-2s">MAKE AN APPOINTMENT</button>
        </div>
      </div>
    </slide>
    <slide class="slide2">
      <div class="container">
        <div class="slide-title">
            <h4 class="slide-title-h4 wow slideInUp delay-2s">A range of programs for women's healthcare</h4>
            <h1 class="slide-title-h1 wow slideInUp delay-2s">Special Touch</h1>
            <button class="slide-title-button button wow slideInUp delay-2s">MAKE AN APPOINTMENT</button>
        </div>
      </div>
    </slide>
    <slide class="slide3">
      <div class="container">
        <div class="slide-title">
            <h4 class="slide-title-h4 wow slideInUp delay-2s">A range of programs for women's healthcare</h4>
            <h1 class="slide-title-h1 wow slideInUp delay-2s">Special Touch</h1>
            <button class="slide-title-button button wow slideInUp delay-2s">MAKE AN APPOINTMENT</button>
        </div>
      </div>
    </slide>

    <hooper-navigation slot="hooper-addons"></hooper-navigation>
  </hooper>
</template>

<script>
import { Hooper, Slide } from 'hooper';
import 'hooper/dist/hooper.css';
  import {
  Navigation as HooperNavigation
  } from 'hooper';

export default {
  components: {
    Hooper,
    Slide,
    HooperNavigation
  }
}
</script>
<style lang="scss" scoped> 
   $color-page: #00BB6D;
   %slider-title{
     outline: none;
      padding-left: 10%;
      display: flex;
      align-items: center;
      width: 100%;
      white-space: normal;
   }
   .button:before {
     background: #2f353e;
   }
    .hooper{
        position: relative;
       -webkit-box-sizing: border-box;
        box-sizing: border-box;
        width: 100%;
        height: calc(100vh - 170px);
    }
    .slide1{
      background: url('../../assets/slide-01.jpg')100% 100% no-repeat;
      @extend %slider-title;
      background-size: cover;
    }
    .slide2{
      background: url('../../assets/slide-02.jpg')100% 100% no-repeat;
      @extend %slider-title;
      background-size: cover;
    }
    .slide3{
      background: url('../../assets/slide-03.jpg')100% 100% no-repeat;
      @extend %slider-title;
      background-size: cover;
    }
    .hooper-track {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    height: 100%;
    .hooper-navigation {
      .hooper-prev {
         background-color: white !important;
        &:hover{
          color: white;
          background: $color-page;
          .icon-arrowLeft {
          fill: #fff;
          }
          .icon-arrowRight {
          fill: #fff;
          }
        }
      }
      .hooper-next {
         background-color: white !important;
        &:hover{
          color: white;
          background: $color-page;
          .icon-arrowLeft {
          fill: #fff;
          }
          .icon-arrowRight {
          fill: #fff;
          }
        }
      }
    }
  }
  .hooper-liveregion {
    display: none;
  }
  .hooper-prev {
    position: absolute;
    left: 180px;
    bottom: unset;
    top: 50%;
    margin-top: -41px;
    transform: translateY(-50%);
    border-radius: 50%;
    padding: 5px 7px;
    background-color: transparent;
    border: 2px solid rgba(255, 255, 255, .8);
    color: #fff;
    &:hover {
      cursor: pointer;
    }
    .icon-arrowLeft {
      fill: #fff;
    }
  }
  .hooper-list {
    overflow: hidden;
  }
  .hooper-next {
    position: absolute;
    right: 180px;
    bottom: unset;
    top: 50%;
    margin-top: -41px;
    transform: translateY(-50%);
    padding: 5px 7px;
    border-radius: 50%;
    background-color: transparent;
    color: #fff;
    border: 2px solid rgba(255, 255, 255, .8);
    &:hover {
      cursor: pointer;
    }
    .icon-arrowRight {
      fill: #fff;
    }
  }
    // .hooper-navigation {
    //   .hooper-liveregion {
    //     display: none;
    //   }
    //   .hooper-prev {
    //   background: white;
    //   &:hover{
    //     color: white;
    //     background: $color-page;
    //     .icon-arrowLeft {
    //     fill: #fff;
    //     }
    //     .icon-arrowRight {
    //     fill: #fff;
    //     }
    //   }
    // }
    // .hooper-next {
    //   background: white;
    //   &:hover{
    //     color: white;
    //     background: $color-page;
    //     .icon-arrowLeft {
    //     fill: #fff;
    //     }
    //     .icon-arrowRight {
    //     fill: #fff;
    //     }
    //   }
    //  }
    // }
    .hooper-next, .hooper-prev {
      background: white;
      &:hover{
        color: white;
        background: $color-page;
        .icon-arrowLeft {
        fill: #fff;
        }
        .icon-arrowRight {
        fill: #fff;
        }
      }
    }
    .slide-title{
      padding: 90px 0 140px;
      animation: shimmy 1s ;
      animation-direction: alternate;
    }
     @keyframes shimmy {
        100% {
            transform: translate(0, 0);    
        }
        0% {
            transform: translate(0, 100px);
        }
        }
    .fixed{
        display: block;
        
    }
    .slide-title-h4{
          padding-left: 22px;
          line-height: 1.2;
          font-size: 20px;
          border-left: 4px solid $color-page;
          color: #151515;
          letter-spacing: 0.1em;
        }
    .slide-title-h1{
          font-family: 'Montserrat', sans-serif;
          font-weight: 400;
          letter-spacing: .1em;
          font-size: 38px;
          color: #151515;
          line-height: 1.2;
          margin-top: 25px;
         
    }    
    .slide-title-button{
          background: $color-page;
          color: white;
          border: none;
          font-size: 12px;
          text-align: center;
          padding: 9px 30px;
          min-height: 51px;
          min-width: 180px;
          margin-top: 30px;
        }
       
    @media (max-width: 1030px) {
      .slide-title-h4{
        font-size: 20px;
      }
      .slide-title-h1{
        font-size: 38px;
      }
      .slide1{
      background: none;
      background-size: cover;
      position: relative;
      &::before{
        content: '';
        position: absolute;
        top: 0;
        left: 0;
        background-color: #fff;
         background: url('../../assets/slide-01.jpg')100% 100% no-repeat;
         background-size: cover;
         opacity: 0.5;
         height: 100%;
         width: 100%;
      }
    }
    .slide2{
     background: none;
      background-size: cover;
      position: relative;
      &::before{
        content: '';
        position: absolute;
        top: 0;
        left: 0;
        background-color: #fff;
         background: url('../../assets/slide-02.jpg')100% 100% no-repeat;
         background-size: cover;
         opacity: 0.5;
         height: 100%;
         width: 100%;
      }
    }
    .slide3{
      background: none;
      background-size: cover;
      position: relative;
      &::before{
        content: '';
        position: absolute;
        top: 0;
        left: 0;
        background-color: #fff;
         background: url('../../assets/slide-03.jpg')100% 100% no-repeat;
         background-size: cover;
         opacity: 0.5;
         height: 100%;
         width: 100%;
      }
    }
    }
    @media (max-width: 775px) {
      // .container{
      //      background: rgba(255,245,215,0.4);
      // }
      // %slider-title{
      //    background: rgba(255,255,255,0.5);
      // }
      .slide-title-h4{
        display: none;
      }
    
    }
    </style>