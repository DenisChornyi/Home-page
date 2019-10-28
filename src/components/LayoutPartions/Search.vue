<template>
  <div class="search">
      <div class="search__box">
           <input type="text" placeholder="Search...">
           <div class="search__box__btn">

           </div>
      </div>
  </div>
</template>

<script>
  export default{
       data() {
        //    return {
        //      isActive : false
        //    }
       },
        methods: {
            isSearch: function(){
                console.log(1)
            }
        }
    }
</script>
<style lang="scss" scoped>
    .active{
        visibility: visible;
        opacity: 1;
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
            margin: 220px auto;
            width: 550px;
            border-bottom: 1px solid white;
            input{
                outline: none;
                background-color: transparent;
                border: none;
                width: 100%;
                height: 50px;
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