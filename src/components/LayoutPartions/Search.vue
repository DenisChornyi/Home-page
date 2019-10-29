<template>

 <div>
     <div class="search" v-bind:class="{active: classSearch}">
      <div class="search__box">
           <input type="text" placeholder="Search...">
           <div class="search__box__btn">
               <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" version="1.1" id="search-btn" x="0px" y="0px" viewBox="0 0 451 451" style="enable-background:new 0 0 451 451;" xml:space="preserve">
                    <g>
                        <path d="M447.05,428l-109.6-109.6c29.4-33.8,47.2-77.9,47.2-126.1C384.65,86.2,298.35,0,192.35,0C86.25,0,0.05,86.3,0.05,192.3   s86.3,192.3,192.3,192.3c48.2,0,92.3-17.8,126.1-47.2L428.05,447c2.6,2.6,6.1,4,9.5,4s6.9-1.3,9.5-4   C452.25,441.8,452.25,433.2,447.05,428z M26.95,192.3c0-91.2,74.2-165.3,165.3-165.3c91.2,0,165.3,74.2,165.3,165.3   s-74.1,165.4-165.3,165.4C101.15,357.7,26.95,283.5,26.95,192.3z"/>
                    </g>

                    </svg>
              <a v-on:click="classSearch=!classSearch"><svg
               xmlns="http://www.w3.org/2000/svg" id="search-btn" width="30" height="30" viewBox="0 0 18 18"><path d="M14.53 4.53l-1.06-1.06L9 7.94 4.53 3.47 3.47 4.53 7.94 9l-4.47 4.47 1.06 1.06L9 10.06l4.47 4.47 1.06-1.06L10.06 9z"/></svg></a>
           </div>
      </div>
  </div>
</div>
 
</template>

<script>

  export default{
        data() {
           return {
             isActive : true
           }
        },
        props: [
            'classSearch'
        ]
    }
</script>
<style lang="scss" scoped>
    .active{
        visibility: visible !important;
        opacity: 1 !important;
    }
    .search{
        // visibility: visible;
        // opacity: 1;
        position: fixed;
        top: 0;
        bottom: 0;
        left: 0;
        right: 0;
        height: 100vh;
        width: 100vw;
        display: flex;
        align-items: flex-start;
        justify-content: center;
        background-color: rgba(23, 23, 23, 0.57);
        opacity: 0;
        visibility: hidden;
        transition: .3s;
        z-index: 20;
        &__box{
            display: flex;
            align-items: center;
            justify-content: space-between;
            &__btn{
                display: flex;
                  align-items: center;
                justify-content: space-between;
                #search-btn{
                    fill: #fff;
                    height: 30px;
                    width: 30px;
                    margin-left: 15px;
                    &:hover{
                        fill: #47c055;
                    }
                }
            }
            margin: 220px auto;
            width: 550px;
            border-bottom: 1px solid white;
            input{
                outline: none;
                background-color: transparent;
                border: none;
                width: 100%;
                height: 50px;
                font-size: 36px;
                color: #fff;
            }
        }
    }
    ::placeholder{
           font-family: "Montserrat", sans-serif;
            font-size: 36px;
            color: #fff;
            letter-spacing: 0.05em;
        }
</style>