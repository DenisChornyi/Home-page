<template>


  <hooper :infiniteScrol="true" :autoPlay="true"  :transition="600" :playSpeed="3500" :wheelControl="false">
    <slide class="slide1">
      <div class="slide-title">
          <h4 class="slide-title-h4">A range of programs for women's healthcare</h4>
          <h1 class="slide-title-h1">Special Touch</h1>
          <button class="slide-title-button">MAKE AN APPOINTMENT</button>
      </div>
    </slide>
    <slide class="slide2">
      <div class="slide-title">
          <h4 class="slide-title-h4">A range of programs for women's healthcare</h4>
          <h1 class="slide-title-h1">Special Touch</h1>
          <button class="slide-title-button">MAKE AN APPOINTMENT</button>
      </div>
    </slide>
    <slide class="slide3">
      <div class="slide-title">
          <h4 class="slide-title-h4">A range of programs for women's healthcare</h4>
          <h1 class="slide-title-h1">Special Touch</h1>
          <button class="slide-title-button">MAKE AN APPOINTMENT</button>
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
<style lang="scss"> 
   $color-page: #00BB6D;
   %slider-title{
      padding-left: 10%;
      align-items: center;
      display: flex;
      width: 100%;
      white-space: normal;
   }
    .hooper{
        position: relative;
       -webkit-box-sizing: border-box;
        box-sizing: border-box;
        width: 100%;
        height: 37em;
       
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
          font-size: 58px;
          color: #151515;
          line-height: 1.2;
          margin-top: 25px;
          letter-spacing: 0.1em;
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
    </style>