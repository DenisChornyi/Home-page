<template>
    <div class="container">
    <div class="doctors columns">
        <div class="doctors__left column is-four-fifths">
            <div class="doctors__left__title">
                <h2>Our Doctors</h2>
                <div class="doctors__left__title__buttons">
                    <button class="doctors__left__title__buttons__btn button">VIEW TIMETABLE</button>
                </div>
            </div>
            
            <hooper id="hooper" :itemsToShow="4" :wheelControl="false" :infiniteScrol="true">
                <slide id="slide" class="slide-doctor">
                    <img class="slide-doctor__img" src="../../assets/diagnostics-04.jpg" alt="Photo">
                    <div class="slide-doctor__info">
                        <h4>Dr. Max Turner</h4>
                        <p>Cardiology</p>
                        <div class="slide-doctor__info__phone">
                            <svg id="phone" xmlns="http://www.w3.org/2000/svg" xmlns:sketch="http://www.bohemiancoding.com/sketch/ns" xmlns:xlink="http://www.w3.org/1999/xlink" height="18px" version="1.1" viewBox="0 0 18 18" width="18px"><title/><desc/><defs/><g fill="none" fill-rule="evenodd" id="Page-1" stroke="none" stroke-width="1"><g fill="#000000" id="Icons-Communication" transform="translate(-85.000000, -126.000000)"><g id="phone" transform="translate(85.000000, 126.000000)"><path d="M3.6,7.8 C5,10.6 7.4,12.9 10.2,14.4 L12.4,12.2 C12.7,11.9 13.1,11.8 13.4,12 C14.5,12.4 15.7,12.6 17,12.6 C17.6,12.6 18,13 18,13.6 L18,17 C18,17.6 17.6,18 17,18 C7.6,18 0,10.4 0,1 C0,0.4 0.4,0 1,0 L4.5,0 C5.1,0 5.5,0.4 5.5,1 C5.5,2.2 5.7,3.4 6.1,4.6 C6.2,4.9 6.1,5.3 5.9,5.6 L3.6,7.8 L3.6,7.8 Z" id="Shape"/></g></g></g></svg>
                            <a>+1 (409) 987-5874</a>
                        </div>
                    </div>
                </slide>
                 <slide id="slide" class="slide-doctor">
                    <img class="slide-doctor__img" src="../../assets/diagnostics-04.jpg" alt="Photo">
                    <div class="slide-doctor__info">
                        <h4>Dr. Max Turner</h4>
                        <p>Cardiology</p>
                        <div class="slide-doctor__info__phone">
                            <svg id="phone" xmlns="http://www.w3.org/2000/svg" xmlns:sketch="http://www.bohemiancoding.com/sketch/ns" xmlns:xlink="http://www.w3.org/1999/xlink" height="18px" version="1.1" viewBox="0 0 18 18" width="18px"><title/><desc/><defs/><g fill="none" fill-rule="evenodd" id="Page-1" stroke="none" stroke-width="1"><g fill="#000000" id="Icons-Communication" transform="translate(-85.000000, -126.000000)"><g id="phone" transform="translate(85.000000, 126.000000)"><path d="M3.6,7.8 C5,10.6 7.4,12.9 10.2,14.4 L12.4,12.2 C12.7,11.9 13.1,11.8 13.4,12 C14.5,12.4 15.7,12.6 17,12.6 C17.6,12.6 18,13 18,13.6 L18,17 C18,17.6 17.6,18 17,18 C7.6,18 0,10.4 0,1 C0,0.4 0.4,0 1,0 L4.5,0 C5.1,0 5.5,0.4 5.5,1 C5.5,2.2 5.7,3.4 6.1,4.6 C6.2,4.9 6.1,5.3 5.9,5.6 L3.6,7.8 L3.6,7.8 Z" id="Shape"/></g></g></g></svg>
                            <a>+1 (409) 987-5874</a>
                        </div>
                    </div>
                </slide>
               <slide id="slide" class="slide-doctor">
                    <img class="slide-doctor__img" src="../../assets/diagnostics-04.jpg" alt="Photo">
                    <div class="slide-doctor__info">
                        <h4>Dr. Max Turner</h4>
                        <p>Cardiology</p>
                        <div class="slide-doctor__info__phone">
                            <svg id="phone" xmlns="http://www.w3.org/2000/svg" xmlns:sketch="http://www.bohemiancoding.com/sketch/ns" xmlns:xlink="http://www.w3.org/1999/xlink" height="18px" version="1.1" viewBox="0 0 18 18" width="18px"><title/><desc/><defs/><g fill="none" fill-rule="evenodd" id="Page-1" stroke="none" stroke-width="1"><g fill="#000000" id="Icons-Communication" transform="translate(-85.000000, -126.000000)"><g id="phone" transform="translate(85.000000, 126.000000)"><path d="M3.6,7.8 C5,10.6 7.4,12.9 10.2,14.4 L12.4,12.2 C12.7,11.9 13.1,11.8 13.4,12 C14.5,12.4 15.7,12.6 17,12.6 C17.6,12.6 18,13 18,13.6 L18,17 C18,17.6 17.6,18 17,18 C7.6,18 0,10.4 0,1 C0,0.4 0.4,0 1,0 L4.5,0 C5.1,0 5.5,0.4 5.5,1 C5.5,2.2 5.7,3.4 6.1,4.6 C6.2,4.9 6.1,5.3 5.9,5.6 L3.6,7.8 L3.6,7.8 Z" id="Shape"/></g></g></g></svg>
                            <a>+1 (409) 987-5874</a>
                        </div>
                    </div>
                </slide>
                <slide id="slide" class="slide-doctor">
                    <img class="slide-doctor__img" src="../../assets/diagnostics-04.jpg" alt="Photo">
                    <div class="slide-doctor__info">
                        <h4>Dr. Max Turner</h4>
                        <p>Cardiology</p>
                        <div class="slide-doctor__info__phone">
                            <svg id="phone" xmlns="http://www.w3.org/2000/svg" xmlns:sketch="http://www.bohemiancoding.com/sketch/ns" xmlns:xlink="http://www.w3.org/1999/xlink" height="18px" version="1.1" viewBox="0 0 18 18" width="18px"><title/><desc/><defs/><g fill="none" fill-rule="evenodd" id="Page-1" stroke="none" stroke-width="1"><g fill="#000000" id="Icons-Communication" transform="translate(-85.000000, -126.000000)"><g id="phone" transform="translate(85.000000, 126.000000)"><path d="M3.6,7.8 C5,10.6 7.4,12.9 10.2,14.4 L12.4,12.2 C12.7,11.9 13.1,11.8 13.4,12 C14.5,12.4 15.7,12.6 17,12.6 C17.6,12.6 18,13 18,13.6 L18,17 C18,17.6 17.6,18 17,18 C7.6,18 0,10.4 0,1 C0,0.4 0.4,0 1,0 L4.5,0 C5.1,0 5.5,0.4 5.5,1 C5.5,2.2 5.7,3.4 6.1,4.6 C6.2,4.9 6.1,5.3 5.9,5.6 L3.6,7.8 L3.6,7.8 Z" id="Shape"/></g></g></g></svg>
                            <a>+1 (409) 987-5874</a>
                        </div>
                    </div>
                </slide>
                 <slide id="slide" class="slide-doctor">
                    <img class="slide-doctor__img" src="../../assets/diagnostics-04.jpg" alt="Photo">
                    <div class="slide-doctor__info">
                        <h4>Dr. Max Turner</h4>
                        <p>Cardiology</p>
                        <div class="slide-doctor__info__phone">
                            <svg id="phone" xmlns="http://www.w3.org/2000/svg" xmlns:sketch="http://www.bohemiancoding.com/sketch/ns" xmlns:xlink="http://www.w3.org/1999/xlink" height="18px" version="1.1" viewBox="0 0 18 18" width="18px"><title/><desc/><defs/><g fill="none" fill-rule="evenodd" id="Page-1" stroke="none" stroke-width="1"><g fill="#000000" id="Icons-Communication" transform="translate(-85.000000, -126.000000)"><g id="phone" transform="translate(85.000000, 126.000000)"><path d="M3.6,7.8 C5,10.6 7.4,12.9 10.2,14.4 L12.4,12.2 C12.7,11.9 13.1,11.8 13.4,12 C14.5,12.4 15.7,12.6 17,12.6 C17.6,12.6 18,13 18,13.6 L18,17 C18,17.6 17.6,18 17,18 C7.6,18 0,10.4 0,1 C0,0.4 0.4,0 1,0 L4.5,0 C5.1,0 5.5,0.4 5.5,1 C5.5,2.2 5.7,3.4 6.1,4.6 C6.2,4.9 6.1,5.3 5.9,5.6 L3.6,7.8 L3.6,7.8 Z" id="Shape"/></g></g></g></svg>
                            <a>+1 (409) 987-5874</a>
                        </div>
                    </div>
                </slide>
                <slide id="slide" class="slide-doctor">
                    <img class="slide-doctor__img" src="../../assets/diagnostics-04.jpg" alt="Photo">
                    <div class="slide-doctor__info">
                        <h4>Dr. Max Turner</h4>
                        <p>Cardiology</p>
                        <div class="slide-doctor__info__phone">
                            <svg id="phone" xmlns="http://www.w3.org/2000/svg" xmlns:sketch="http://www.bohemiancoding.com/sketch/ns" xmlns:xlink="http://www.w3.org/1999/xlink" height="18px" version="1.1" viewBox="0 0 18 18" width="18px"><title/><desc/><defs/><g fill="none" fill-rule="evenodd" id="Page-1" stroke="none" stroke-width="1"><g fill="#000000" id="Icons-Communication" transform="translate(-85.000000, -126.000000)"><g id="phone" transform="translate(85.000000, 126.000000)"><path d="M3.6,7.8 C5,10.6 7.4,12.9 10.2,14.4 L12.4,12.2 C12.7,11.9 13.1,11.8 13.4,12 C14.5,12.4 15.7,12.6 17,12.6 C17.6,12.6 18,13 18,13.6 L18,17 C18,17.6 17.6,18 17,18 C7.6,18 0,10.4 0,1 C0,0.4 0.4,0 1,0 L4.5,0 C5.1,0 5.5,0.4 5.5,1 C5.5,2.2 5.7,3.4 6.1,4.6 C6.2,4.9 6.1,5.3 5.9,5.6 L3.6,7.8 L3.6,7.8 Z" id="Shape"/></g></g></g></svg>
                            <a>+1 (409) 987-5874</a>
                        </div>
                    </div>
                </slide>
                <hooper-navigation slot="hooper-addons"></hooper-navigation>
            </hooper>
        </div>
        <div class="doctors__right column">
            <div class="doctors__right__images">
                <a>Make an<br> Appointment</a>
                <p>let up help you deal with<br> health concerns.</p>
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
  }
}
</script>
<style lang="scss" scoped> 
@import url('https://fonts.googleapis.com/css?family=Roboto&display=swap');
   $color-page: #00BB6D;
    .doctors{
        padding: 50px 10px 90px;
        display: flex;
       justify-content: space-between;
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
                border-bottom: 1px solid #ebebeb;
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
       &__right{
            &__images{
                background: url('../../assets/about-02-268x483.jpg')100% 100% no-repeat;
                background-size: cover;
                max-width: 268px;
                max-height: 500px;
                text-align: center;
                padding: 300px 0 55px 0;
                a{
                    font-size: 20px;
                    color: #fff;
                }
                p{
                    margin-top:10px;
                    color: #fff;
                }
                &:hover{
                    background-size: 105% auto;
                    color: #fff;
                    a{
                        text-decoration: underline;
                        color: #fff;
                    }
                }
            }
       }
    }
    #slide{
        width: 25%;
        padding: 10px;
    }
    .slide-doctor{
        max-height: 363px;
        max-width: 258px;
        margin: 0 10px;
        
       &__img{
            max-height: 208px;
            max-width: 258px;
            margin: 0;
       }
       &__info{
            max-width: 268px;
            margin-top: -6px;
            padding: 22px 40px 28px;
            background-color: #2F4858;
            transition: .3s ease-out background-color;
            text-align: center;
            color: #fff;
            p{
                font-size: 14px;
                color: $color-page;
                margin: 0 auto;
                width: 120px;
                padding: 5px 0 10px;
                border-bottom: 1px solid #9b9b9b;
                margin-bottom: 10px;
            }
            h4{
                line-height: 1.441;
                color: #fff;
                font-size: 18px;
            }
            &__phone{
                    #phone{
                        fill: $color-page;
                        height: 15px;
                        margin-right: 10px;
                    }
                    a{
                        color: #fff;
                    }
            }
       }
    }

    #hooper{
        height: 100%;
        
    }
    #slide{
        width: 25%;
        padding: 10px;
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
     .doctors{
         flex-direction: row;
    }
}
@media (max-width: 1030px) {
    .doctors__right{
         width: 280px;
    }
    .doctors{
         align-items: center;
         flex-direction: column;
          &__left{
            width:100%;
                  
        }
    }
    .hooper-slide{
        width: 33%;
        padding: 15px;
    }
    .is-four-fifths{
        width: 100% !important;
    }
    .slide-doctor__info{
            padding:22px 20px;    
    }
}
    @media (max-width: 700px) {
        .doctors{
            flex-direction: column;
        &__left{
            width:100%;
            &__title{
                flex-direction: column;
                align-items: center;
            }
        }
        &__right{
           width: 268px;
             height: 483px;
            margin: 0 auto;
        }
    } 
        .hooper-slide{
            width: 33%;
            padding: 15px;
        }

    }
    
</style>