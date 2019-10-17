<template>
    <div class="departments">
        <div class="departments1">
            <div class="departments1-title">
                <h2>Departments</h2>
                <div class="departments1-title-buttons">
                    <button class="departments1-title-buttons_btn">ALL DEPARTMENS</button>
                </div>
            </div>
            
            <hooper id="hooper" :itemsToShow="4">
                <slide id="slide">
                    <img class="depart-img" src="../../assets/departments1.jpg" alt="Photo">
                    <div class="slide-info">
                        <div class="slide-info-line"></div>
                        <h4>Neurology</h4>
                    </div>
                    <p>Providing quality primary, secondary and tertiary childcare.</p>
                </slide>
                <slide id="slide">
                    <img class="depart-img" src="../../assets/departments1.jpg" alt="Photo">
                    <div class="slide-info">
                        <div class="slide-info-line"></div>
                        <h4>Neurology</h4>
                    </div>
                    <p>Providing quality primary, secondary and tertiary childcare.</p>
                </slide>
                <slide id="slide">
                    <img class="depart-img" src="../../assets/departments1.jpg" alt="Photo">
                    <div class="slide-info">
                        <div class="slide-info-line"></div>
                        <h4>Neurology</h4>
                    </div>
                    <p>Providing quality primary, secondary and tertiary childcare.</p>
                </slide>
                <slide id="slide">
                    <img class="depart-img" src="../../assets/departments1.jpg" alt="Photo">
                    <div class="slide-info">
                        <div class="slide-info-line"></div>
                        <h4>Neurology</h4>
                    </div>
                    <p>Providing quality primary, secondary and tertiary childcare.</p>
                </slide>
                <slide id="slide">
                    <img class="depart-img" src="../../assets/departments1.jpg" alt="Photo">
                    <div class="slide-info">
                        <div class="slide-info-line"></div>
                        <h4>Neurology</h4>
                    </div>
                    <p>Providing quality primary, secondary and tertiary childcare.</p>
                </slide>
                <slide id="slide">
                    <img class="depart-img" src="../../assets/departments1.jpg" alt="Photo">
                    <div class="slide-info">
                        <div class="slide-info-line"></div>
                        <h4>Neurology</h4>
                    </div>
                    <p>Providing quality primary, secondary and tertiary childcare.</p>
                </slide>
                <hooper-navigation slot="hooper-addons"></hooper-navigation>
            </hooper>
        </div>
        <div class="departments2">
            <div class="departments2-buttons">
                <button class="departments2-buttons_btn">NEUROLOGY</button>
                <button class="departments2-buttons_btn">TRAUMATOLOGY</button>
                <button class="departments2-buttons_btn">DENTISTRY</button>
                <button class="departments2-buttons_btn">CARDIOLOGY</button>
                <button class="departments2-buttons_btn">OPHALMOLOGY</button>
                <button class="departments2-buttons_btn">PEDIATRICS</button>
            </div>
        </div>
    </div>
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
    .departments{
        padding: 90px 15px;
        display: flex;
       align-items: center;
       justify-content: space-between;
    }
    .departments2{
        width:17%;
    }
    .departments2-buttons{
        display: flex;
        flex-direction: column;
    }
    .departments2-buttons_btn{
        background: #2F4858;
        padding: 25px 10px;
        color: #fff;
        border: none;
        border-bottom: 0.5px solid #9b9b9b;
        font-size: 16px;
        &:hover{
            color: $color-page;
        }
    }
    .departments1{
    width: 80%;
        h2{
            font-size: 50px;
            color: black;
            
        }
    }
    .departments1-title{
        display: flex;
       align-items: center;
       justify-content: space-between;
       border-bottom: 1px solid #9b9b9b;
       margin-bottom: 20px;
       padding: 20px 0;
        
    }
    #hooper{
        height: 330px;
        
    }
    #slide{
        width: 150px;
        height: 250px;
        &:hover{
            .slide-info-line{
                width: 60px;
            }
        }
    }
    .depart-img{
        height: 229;
        width: 267;
    }
    .slide-info{
        display: flex;
       justify-content: row;
       font-size: 20px;
    }
    .slide-info-line{
        height: 5px;
        transition-duration: 0.5s;
        width: 30px;
        border-top: 5px solid #47c055;
        margin-top:13px;
        margin-right:13px;
    }
    .departments1-title-buttons{
        position: relative;
    }
    .departments1-title-buttons_btn{
        font-size: 12px;
        border: none;
        letter-spacing: 0.05em;
        padding: 9px 15px;
        text-transform: uppercase;
        min-width: 180px;
        min-height: 51px;

    }
//     .hooper-prev {
//     position: absolute;
//     left: 480px;
//     bottom: unset;
//     top: 50%;
//     margin-top: -41px;
//     transform: translateY(-50%);
//     padding: 5px 7px;
//     background-color: transparent;
//     border: 2px solid rgba(255, 255, 255, .8);
//     color: #fff;
//     &:hover {
//       cursor: pointer;
//     }
//     .icon-arrowLeft {
//       fill: #fff;
//     }
//   }
//   .hooper-next {
//     position: absolute;
//     right: 180px;
//     bottom: unset;
//     top: -50%;
//     margin-top: -41px;
//     transform: translateY(-50%);
//     padding: 5px 7px;
//     background-color: transparent;
//     color: #fff;
//     border: 2px solid rgba(255, 255, 255, .8);
//     &:hover {
//       cursor: pointer;
//     }
//     .icon-arrowRight {
//       fill: #fff;
//     }
//   }
</style>