<template>
  <div class="menu">
    <a class="logo" href="index.html"><img class="logo-img" src="../../assets/logo.png" alt="logo"></a>
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
    <svg class="menu-search" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" version="1.1" id="Capa_1" x="0px" y="0px" viewBox="0 0 451 451" style="enable-background:new 0 0 451 451;" xml:space="preserve">
<g>
	<path d="M447.05,428l-109.6-109.6c29.4-33.8,47.2-77.9,47.2-126.1C384.65,86.2,298.35,0,192.35,0C86.25,0,0.05,86.3,0.05,192.3   s86.3,192.3,192.3,192.3c48.2,0,92.3-17.8,126.1-47.2L428.05,447c2.6,2.6,6.1,4,9.5,4s6.9-1.3,9.5-4   C452.25,441.8,452.25,433.2,447.05,428z M26.95,192.3c0-91.2,74.2-165.3,165.3-165.3c91.2,0,165.3,74.2,165.3,165.3   s-74.1,165.4-165.3,165.4C101.15,357.7,26.95,283.5,26.95,192.3z"/>
</g>

</svg>
 </div>
</template>

<script>

</script>
<style lang="scss"> 
   $color-page: #47c055;
    .menu{
        padding: 40px 15px;
        display: flex;
        align-items: center;
        justify-content: space-between;
        transition: .3s ease-out all;
    }
    .navbar{
        display: flex;
        align-items: center;
        justify-content: space-between;
        
    }
    .navbar-menu{
        padding-left: 15%;
        margin: 0 auto;
        width: 700px;
    }
    .navbar-item{
        margin-left: 51px;
        transition: .25s;
        font-weight: 400;
        color: #001515;
        line-height: 1.2;
        font-size: 16px;
    }
    .navbar-item.is-active{
        color: $color-page;
    }
    .logo{
        height: 92px;
        width: 79px;
    
    }
    .logo-img{
        height: 92px;
        width: 79px;
    }
    .menu-search{
        width: 25px;
        height: 25px;
        font-size: 24px;
        &:hover{
            fill: $color-page;
        }
    }
    #link-hover{
        &:hover{
            color: $color-page;
            background: transparent;
        }
        &:active{
            color: $color-page;
        }
        &:first-child{
           
        }
    }
</style>