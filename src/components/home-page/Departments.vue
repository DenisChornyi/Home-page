<template>
    <div class="container">
    <div class="departments columns">
        <div class="departments__left column is-four-fifths">
            <div class="departments__left__title">
                <h2>Departments</h2>
                <div class="departments__left__title__buttons">
                    <button class="departments__left__title__buttons__btn button">ALL DEPARTMENS</button>
                </div>
            </div>
            
            <hooper id="hooper" :settings="hooperSettings">
                <slide id="slide">
                    <img class="depart-img" src="../../assets/departments1.jpg" alt="Photo">
                    <div class="slide__info">
                        <div class="slide__info__line"></div>
                        <h4>Neurology</h4>
                    </div>
                    <p>Providing quality primary, secondary and tertiary childcare.</p>
                </slide>
                <slide id="slide">
                    <img class="depart-img" src="../../assets/departments1.jpg" alt="Photo">
                   <div class="slide__info">
                        <div class="slide__info__line"></div>
                        <h4>Neurology</h4>
                    </div>
                    <p>Providing quality primary, secondary and tertiary childcare.</p>
                </slide>
                <slide id="slide">
                    <img class="depart-img" src="../../assets/departments1.jpg" alt="Photo">
                    <div class="slide__info">
                        <div class="slide__info__line"></div>
                        <h4>Neurology</h4>
                    </div>
                    <p>Providing quality primary, secondary and tertiary childcare.</p>
                </slide>
                <slide id="slide">
                    <img class="depart-img" src="../../assets/departments1.jpg" alt="Photo">
                    <div class="slide__info">
                        <div class="slide__info__line"></div>
                        <h4>Neurology</h4>
                    </div>
                    <p>Providing quality primary, secondary and tertiary childcare.</p>
                </slide>
                <slide id="slide">
                    <img class="depart-img" src="../../assets/departments1.jpg" alt="Photo">
                    <div class="slide__info">
                        <div class="slide__info__line"></div>
                        <h4>Neurology</h4>
                    </div>
                    <p>Providing quality primary, secondary and tertiary childcare.</p>
                </slide>
                <slide id="slide">
                    <img class="depart-img" src="../../assets/departments1.jpg" alt="Photo">
                    <div class="slide__info">
                        <div class="slide__info__line"></div>
                        <h4>Neurology</h4>
                    </div>
                    <p>Providing quality primary, secondary and tertiary childcare.</p>
                </slide>
                <hooper-navigation slot="hooper-addons"></hooper-navigation>
            </hooper>
        </div>
        <div class="departments__right column">
            <div class="departments__right__buttons">
                <button class="departments__right__buttons__btn">NEUROLOGY</button>
                <button class="departments__right__buttons__btn">TRAUMATOLOGY</button>
                <button class="departments__right__buttons__btn">DENTISTRY</button>
                <button class="departments__right__buttons__btn">CARDIOLOGY</button>
                <button class="departments__right__buttons__btn">OPHALMOLOGY</button>
                <button class="departments__right__buttons__btn">PEDIATRICS</button>
            </div>
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
  },
  data() {
    return {
      hooperSettings: {
           itemsToShow: 4,
           wheelControl: false,
           infiniteScrol: true,
           breakpoints: {
            1000: {
                itemsToShow: 3
            },
            430:{
                itemsToShow: 1
            }
        }
      }
    }
}
}
</script>
<style lang="scss" scoped> 
@import url('https://fonts.googleapis.com/css?family=Montserrat&display=swap');
   $color-page: #00BB6D;
    .departments{
        padding: 90px 15px;
        display: flex;
       justify-content: space-between;
       &__right{
            &__buttons{
                display: flex;
                flex-direction: column;
                &__btn{
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
            }
            
        }
        &__left{
                h2{
                    font-family: "Montserrat", sans-serif;
                    font-weight: 400;
                    letter-spacing: 0.05em;
                    color: #151515;
                    font-size: 32px;
                }
                &__title{
                    display: flex;
                    justify-content: space-between;
                    border-bottom: 1px solid #ebebeb;;
                    margin-bottom: 20px;
                    padding-bottom: 20px;
                    &__buttons{
                        &__btn{
                            color: #151515;
                            background-color: #ebebeb;
                            font-size: 12px;
                            border: none;
                            letter-spacing: 0.05em;
                            padding: 9px 15px;
                            text-transform: uppercase;
                            min-width: 180px;
                            min-height: 51px;

                        }
                    }
                }
            }
    }
  
    #hooper{
        height: 330px;
        
    }
    #slide{
        width: 25%;
        padding: 10px;
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
    .slide__info{
        display: flex;
       justify-content: row;
       font-size: 20px;
       &__line{
            height: 5px;
            transition-duration: 0.5s;
            width: 30px;
            border-top: 5px solid #47c055;
            margin-top:13px;
            margin-right:13px;
        }
    }
@media (max-width: 2600px) {
        .container{
            max-width: 1500px;
        }
    }
@media (max-width: 1444px) {
        .container{
            max-width: 100%;
        }
        .departments{
        flex-direction: row;
    }
    }
@media (max-width: 1030px) {
    .departments{
        flex-direction: column;
        &__left{
             width:100%;
        }
        &__right{
            width:26%;
        }
    }
    #slide{
        width: 33%;
        padding: 15px;
    }
    .is-four-fifths{
        width: 100% !important;
    }
    
    }
    @media (max-width: 700px) {
    .departments{
        align-items: center;
        &__left{
            width:100%;
            &__title{
                flex-direction: column;
                align-items: center;
            }
        }
        &__right{
             width:60%;
        }
    } 
        #slide{
            width: 33%;
            padding: 15px;
        }
        .is-four-fifths{
        width: 100% !important;
    }
    }
</style>