<template>
<div class="menu" :class="{ 'fixed filled': fixed }">
<div class="container"> 
  <div class="menu__contain">
    <a class="menu__contain__logo" href="index.html"><img class="menu__contain__logo-img" src="../../assets/logo.png" alt="logo"></a>
    <div class="navbar-menu">
        <div class="navbar">
            <a id="link-hover" class="navbar-item is-active">
                Home
            </a>
            <a id="link-hover" class="navbar-item">
                About us
            </a>
            <div id="link-hover" class="navbar-item has-dropdown is-hoverable">
                <a id="link-hover" class="navbar-link">Departmens</a>
                <div class="navbar-dropdown">
                     <a id="link-hover" class="navbar-item">
                        Timetable
                     </a>
                     <a id="link-hover" class="navbar-item">
                        Timetable
                     </a>
                     <a id="link-hover" class="navbar-item">
                        Timetable
                     </a>
                     <a id="link-hover" class="navbar-item">
                        Timetable
                     </a>
                     <a id="link-hover" class="navbar-item">
                        Timetable
                     </a>
                </div>
            </div>
            <a id="link-hover" class="navbar-item">
                Timetable
            </a>
            <div class="navbar-item has-dropdown is-hoverable">
                <a id="link-hover" class="navbar-link success">Pages</a>
                <div class="navbar-dropdown">
                     <a id="link-hover" class="navbar-item">
                        Timetable
                     </a>
                     <a id="link-hover" class="navbar-item">
                        Timetable
                     </a>
                     <a id="link-hover" class="navbar-item">
                        Timetable
                     </a>
                     <a id="link-hover" class="navbar-item">
                        Timetable
                     </a>
                     <a id="link-hover" class="navbar-item">
                        Timetable
                     </a>
                </div>
            </div>
            <a id="link-hover" class="navbar-item">
                Contacts
            </a>
        </div>
    </div>
    <a><svg class="menu__contain__search" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" version="1.1" id="Capa_1" x="0px" y="0px" viewBox="0 0 451 451" style="enable-background:new 0 0 451 451;" xml:space="preserve">
<g>
	<path d="M447.05,428l-109.6-109.6c29.4-33.8,47.2-77.9,47.2-126.1C384.65,86.2,298.35,0,192.35,0C86.25,0,0.05,86.3,0.05,192.3   s86.3,192.3,192.3,192.3c48.2,0,92.3-17.8,126.1-47.2L428.05,447c2.6,2.6,6.1,4,9.5,4s6.9-1.3,9.5-4   C452.25,441.8,452.25,433.2,447.05,428z M26.95,192.3c0-91.2,74.2-165.3,165.3-165.3c91.2,0,165.3,74.2,165.3,165.3   s-74.1,165.4-165.3,165.4C101.15,357.7,26.95,283.5,26.95,192.3z"/>
</g>

</svg></a>
 </div>
</div>
</div>
</template>

<script>
export default{
       data() {
            return {
                fixed: false,
            };
        },
        methods:{
            isFixed: function() {
                console.log(window.pageYOffset)
                if (window.pageYOffset > 50) {
                this.fixed = true;
                } else {
                this.fixed = false;
                }
            console.log(this.fixed)   
            }
        },    
        mounted() {
            this.isFixed();
            document.addEventListener('scroll', this.isFixed);
                     
        }
    }
</script>
<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css?family=Roboto&display=swap'); 
   $color-page: #47c055;
   .container{
       max-width: 1400px;
       margin: 0 auto;
   }
   .fixed{
       position: fixed;
        z-index: 6;
        top: 0; 
         .menu__contain{ 
             padding: 10px;
             &__logo{
                height: 52px;
                width: 49px;
                &-img{
            height: 52px;
                width: 49px;
                    }
            }
         }      
   }
   .menu{
       width: 100%;
        z-index: 6;
         
        top: 0; 
         background-color: #fff;
   }
    .menu__contain{
        padding: 40px 0;
        display: flex;
        align-items: center;
        justify-content: space-between;
        transition: .3s ease-out all;
            &__logo{
                height: 92px;
                width: 79px;
                &-img{
            height: 92px;
            width: 79px;
                    }
            }
            &__search{
            width: 25px;
            height: 25px;
            font-size: 24px;
            &:hover{
                fill: $color-page;
            }
        }
    }
    .navbar{
        display: flex;
        align-items: center;
        justify-content: space-between;
         margin: 0 auto;
         max-width: 650px;
        
    }
    .navbar-item{
        transition: .25s;
        font-weight: 400;
        color: #001515;
        line-height: 1.2;
        font-size: 16px;
        a{
             color: #001515;
        }
    }
    .navbar-item.is-active{
        color: $color-page;
    }
    #link-hover{
        &:hover{
            color: $color-page;
            background: transparent;
        }
        &:active{
            color: $color-page;
        }
    }
    @media (max-width: 2600px) {
        .container{
            max-width: 1500px;
        }
    }
     @media (max-width: 1444px) {
         .container{
             max-width: 95%;
         }
    }
    @media (max-width: 1030px) {
        .container{
             max-width: 95%;
         }
    }
    @media (max-width: 775px) {
        .menu{
            padding: 10px;
        }
        .logo{
            height: 40px;
        }
         .logo-img{
        height: auto;
        width: 37px;
        }
        .menu-search{
            height: 25px;
            width: 25px;
        }
        }
</style>