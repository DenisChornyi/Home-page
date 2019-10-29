<template>
    <div class="Client">
        <div class="container">
            <div class="client-say">
                <h1>What Our Clients Say</h1>
            </div>
            <div class="client-say">
                <hooper :settings="hooperSettings">
                    <slide>
                        <div class="client-say__slide">
                            <img src="../../assets/clients-say-1.jpg" alt="Photo">
                            <p>
                                I wanted to send enormous thanks for the caring service. It was discreet, diverse and helped me in ways I wasn’t expecting. I was very lucky to have been treated by you. Thank you very much!
                            </p>
                            <h3>Jane Anderson</h3>
                        </div>
                    </slide>
                    <slide>
                        <div class="client-say__slide">
                             <img src="../../assets/clients-say-1.jpg" alt="Photo">
                            <p>
                                I wanted to send enormous thanks for the caring service. It was discreet, diverse and helped me in ways I wasn’t expecting. I was very lucky to have been treated by you. Thank you very much!
                            </p>
                            <h3>Jane Anderson</h3>
                        </div>
                    </slide>
                    <slide>
                        <div class="client-say__slide">
                             <img src="../../assets/clients-say-1.jpg" alt="Photo">
                            <p>
                                I wanted to send enormous thanks for the caring service. It was discreet, diverse and helped me in ways I wasn’t expecting. I was very lucky to have been treated by you. Thank you very much!
                            </p>
                            <h3>Jane Anderson</h3>
                        </div>
                    </slide>
                    <slide>
                        <div class="client-say__slide">
                             <img src="../../assets/clients-say-1.jpg" alt="Photo">
                            <p>
                                I wanted to send enormous thanks for the caring service. It was discreet, diverse and helped me in ways I wasn’t expecting. I was very lucky to have been treated by you. Thank you very much!
                            </p>
                            <h3>Jane Anderson</h3>
                        </div>
                    </slide>
                    <hooper-pagination slot="hooper-addons"></hooper-pagination>
                </hooper>
            </div>
        </div>
    </div>
</template>

<script>
    import { Hooper, Slide } from 'hooper';
    import 'hooper/dist/hooper.css';
    import {
    Pagination as HooperPagination
    } from 'hooper';

    export default {
    components: {
        Hooper,
        Slide,
        HooperPagination
  },
  data() {
    return {
      hooperSettings: {
           itemsToShow: 3,
           wheelControl: false,
           centerMode: true,
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
@import url('https://fonts.googleapis.com/css?family=Roboto&display=swap'); 
   $color-page: #00BB6D;
    .Client{
        background-color: #f2f3f8;
        padding: 90px 15px;
    }
    .client-say{
        text-align: center;
        align-items: center;
        h1{
            font-family: "Montserrat", sans-serif;                
            font-weight: 400;
            letter-spacing: 0.05em;
            color: #151515;
            font-size: 32px;
            margin-bottom: 20px;
        }
    }
    .hooper{
        padding-top: 20px; 
         height: 550px;
          outline: none;
    }
    .hooper-slide.is-active{
        transform: scale(0.9);
        height: 430px;
        opacity: 0.5 !important;
        width: 490px !important;
        transition: transform 1s;
    }
    .hooper-slide.is-active.is-current{
        transform: scale(1);
        opacity: 1 !important;
        z-index: 3;
        margin: 0 -50px;
    }
    ul.hooper-track{
         display: flex;
        align-items: center !important;
    }
    .hooper-list{
        .hooper-track{
             display: flex;
            align-items: center !important;
            .hooper-slide{
                opacity: 0;
                background-color: #fff;
                padding: 20px;
               
                .client-say__slide{
                    display: flex;
                    flex-direction: column;
                    align-items: center;
                    padding: 45px 30px;
                    width: 100%;
                    height: 100%;
                    border: 1px solid #ebebeb;
                    img{
                        border-radius: 50%;
                        box-shadow: 0 4px 7px 0 rgba(0, 0, 0, 0.09);
                        margin-bottom: 30px;
                    }
                    p{
                       font-family: "Roboto", Helvetica, Arial, sans-serif;
                        font-size: 16px;
                        line-height: 1.71429;
                        font-weight: 400;
                        letter-spacing: 0.05em;
                        color: #9b9b9b;
                         margin-bottom: 30px;
                    }
                }
            }
        }
    }.hooper-sr-only{
         height: 9px;
                width: 9px;
                outline: none !important;
                line-height: 0;
                font-size: 0;
                color: transparent;
                padding: 0;
                border-radius: 50%;
                background-color: #9b9b9b;
                border: 0;
                transition: .3s ease-out all;
                cursor: pointer;
    }
    // .hooper-indicator{
    //            height: 9px;
    //             width: 9px;
    //             outline: none !important;
    //             line-height: 0;
    //             font-size: 0;
    //             color: transparent;
    //             padding: 0;
    //             border-radius: 50%;
    //             background-color: #9b9b9b;
    //             border: 0;
    //             transition: .3s ease-out all;
    //             cursor: pointer;
    //         }
    .hooper-pagination{
        .hooper-indicators{
            .hooper-indicator{
               height: 9px;
                width: 9px;
                outline: none !important;
                line-height: 0;
                font-size: 0;
                color: transparent;
                padding: 0;
                border-radius: 50%;
                background-color: #9b9b9b;
                border: 0;
                transition: .3s ease-out all;
                cursor: pointer;
            }
        }
    }
</style>