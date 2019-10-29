<template>
<div class="container">
  <div class="section columns">
    <div class="section-info column">
        <h4>Emergency Help</h4>
        <div class="section-info__phone">
            <svg id="phone" xmlns="http://www.w3.org/2000/svg" xmlns:sketch="http://www.bohemiancoding.com/sketch/ns" xmlns:xlink="http://www.w3.org/1999/xlink" height="18px" version="1.1" viewBox="0 0 18 18" width="18px"><title/><desc/><defs/><g fill="none" fill-rule="evenodd" id="Page-1" stroke="none" stroke-width="1"><g fill="#000000" id="Icons-Communication" transform="translate(-85.000000, -126.000000)"><g id="phone" transform="translate(85.000000, 126.000000)"><path d="M3.6,7.8 C5,10.6 7.4,12.9 10.2,14.4 L12.4,12.2 C12.7,11.9 13.1,11.8 13.4,12 C14.5,12.4 15.7,12.6 17,12.6 C17.6,12.6 18,13 18,13.6 L18,17 C18,17.6 17.6,18 17,18 C7.6,18 0,10.4 0,1 C0,0.4 0.4,0 1,0 L4.5,0 C5.1,0 5.5,0.4 5.5,1 C5.5,2.2 5.7,3.4 6.1,4.6 C6.2,4.9 6.1,5.3 5.9,5.6 L3.6,7.8 L3.6,7.8 Z" id="Shape"/></g></g></g></svg>
            <a href="tel:#">1-800-700-6200</a>
        </div>
        <p>We provide 24/7 professional emergency help for all kinds of medical problems.</p>
    </div>
    <div class="section-info column is-two-fifths">
        <h4>Make an Appointment</h4>
        <div class="section-info__block">
            <div id="select" class="select">
                <select id="selected">
                    <option>Select dropdown</option>
                    <option>With options</option>
                </select>
            </div>
            <input class="section-info__block__input" type="tel" placeholder="Phone">
        </div>
        <div class="section-info__block">
            <input class="section-info__block__input"  type="email" placeholder="E-mail">
            <button class="section-info__block__input button">MAKE AN APPOINTMENT</button>
        </div>
    </div>
    <div class="section-info column">
        <h4>Opening Hours</h4>
        <div class="section-info__data">
            <h5>Weekdays</h5>
            <p>8.00 - 20.00</p>
        </div>
        <div class="section-info__data border">
            <h5>Saturday</h5>
            <p>9.30 - 17.30</p>
        </div>
        <div class="section-info__data">
            <h5>Weekdays</h5>
            <p>9.30 - 15.00</p>
        </div>

    </div>
  </div>
</div>
</template>

<script>

</script>
<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css?family=Montserrat&display=swap'); 
   $color-page: #47c055;
   .section{
       padding: 0;
        padding-bottom: 60px;
        display: flex;
        justify-content: space-between;
   }
   .section-info{
    z-index: 5;
    margin: 15px;
    margin-top: -50px;
    padding: 30px 20px;
    background-color: #fff;
    box-shadow: 0 0 3px 0 rgba(42, 42, 42, 0.35);
        h4{
            font-size: 20px;
            font-family: "Montserrat", sans-serif;
            font-weight: 400;
            letter-spacing: 0.05em;
            color: #151515;
            line-height: 1.2;
        }
        p{
            font-family: "Roboto", Helvetica, Arial, sans-serif;
            font-size: 14px;
            line-height: 1.71429;
            font-weight: 400;
            letter-spacing: 0.05em;
            color: #9b9b9b;
        }
        &__phone{
        margin-top: 30px;
        padding-bottom: 20px;
        margin-bottom: 20px;
        width: 80%;
        border-bottom: 1px solid #ebebeb;
        a{
                font-family: "Montserrat", sans-serif;
                font-size: 18px;
                color: #151515;
                :hover{
                    color: $color-page;
                }
            }
        #phone{
            fill: $color-page;
            margin-right: 10px;
            margin-bottom: -5px;
            height:20px;
                
        }
      }
            &__block{
            margin-top: 25px;
            display: flex;
            align-items: center;
            justify-content: space-between;
               
                 #select{
                    margin-left: 10px;
                    margin-right: 10px;
                    height: 100%;
                    width: 50%;
                    border-radius: 0;
                }
                &__input{
                    outline: none;
                    margin-left: 10px;    
                    margin-right: 10px;
                    padding-left: 10px;
                    padding-right: 10px;
                    height: 50px;
                    border: 1px solid #ebebeb;
                    border-radius: 0;
                    width: 50%;
                    }
        }
            &__data{
                width:100%;
                display: flex;
                align-items: center;
                justify-content: space-between;
                padding: 16px 0;
               
                &.border{
                    border-top: 1px solid #ebebeb;
                    border-bottom: 1px solid #ebebeb;
                }
            }
   }

  .columns{
      margin: 0;
  }
 
   #selected{
       padding-left: 10px;
       padding-right: 15px;
       height: 50px;
       width: 100%;
       outline: none;
       border: 1px solid #ebebeb;
       border-radius: 0;
       color: #9b9b9b;
   }
   .select select{
       outline: none;
       height: 100%;
       width:100%;
       border-radius: 0 !important;
       color: #9b9b9b;
   }
   ::placeholder {
        font-size: 15px;
        color: #9b9b9b;
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
         .section{
            padding: 0;
            padding-bottom: 60px;
            display: flex;
            justify-content: space-between !important;
        }
    }
     @media (max-width: 1030px) {
      .section{
             flex-wrap: wrap;
             padding: 15px;
              padding-top: 40px;
         }
      .section-info{
          flex-shrink: 0;
          margin: 0;
          
          &:nth-child(1){
              width: 50%;
              order: 1;
              width: calc(50% - 15px);
              margin-right: 30px; 
          }
          &:nth-child(2){
              width: 100%;
              margin-top: 30px;
              order: 3;
              margin-bottom: 60px;
          }
          &:nth-child(3){
              width: 50%;
              order: 2;
              width: calc(50% - 15px);
          }
          &__block__input{
                width: 50%;
            }
      }
   #select{
       width: 50%;
   }
    }
    @media (max-width: 800px) {
      .section{
             flex-wrap: wrap;
             padding: 15px;
              padding-top: 40px;
         }
      .section-info{
          flex-shrink: 0;
          margin: 0;
          
          &:nth-child(1){
              width: 50%;
              order: 1;
              width: calc(50% - 15px);
              margin-right: 30px; 
          }
          &:nth-child(2){
              width: 100%;
              margin-top: 30px;
              order: 3;
              margin-bottom: 60px;
              min-width: 650px;
          }
          &:nth-child(3){
              width: 50%;
              order: 2;
              width: calc(50% - 15px);
          }
          &__block__input{
                width: 50%;
            }
      }
   #select{
       width: 50%;
   }
    }
    @media (max-width: 700px) {
      .section{
             flex-direction: column;
              padding-top: 40px;
         }
      .section-info{
          h4{
              margin-bottom: 30px;
          }
          flex-shrink: 0;
          margin: 0;
          
          &:nth-child(1){
              width: 100%;
              order: 1;
          }
          &:nth-child(2){
              width: 100%;
              margin-top: 20px;
              order: 3;
              min-width: 100%;
          }
          &:nth-child(3){
               margin-top: 20px;
              width: 100%;
              order: 2;
          }
          &__block{
              margin-top: 0;
              flex-direction: column;
                &__input{
                width: 100%;
                margin-top: 20px;
            }
             #select{
            width: 100%;
        }
          }
         
            &__data{
                 width: 100%;
        }
        &__phone{
                width: 100%;
            }
      }
        #select{
            width: 100%;
        }
    }
</style>