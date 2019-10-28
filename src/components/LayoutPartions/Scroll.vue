<template>
    <a class="scroll" :class="{ 'fixed filled': fixed }" v-scroll-to="'#menu'">
    </a>
</template>

<script>
   export default{
       data() {
            return {
                fixed: false,
            };
        },
        methods:{
            isScroll: function() {
                if (window.pageYOffset > 150) {
                this.fixed = true;
                } else {
                this.fixed = false;
                }
            
            }
        },    
        mounted() {
            this.isScroll();
            document.addEventListener('scroll', this.isScroll);
                     
        }
    }
</script>
<style lang="scss" scoped> 
    .scroll{
        display: none;
        width: 50px;
        height: 50px;
        font-size: 24px;
        line-height: 46px;
        color: #FFF;
        background: #00BB6D;
        border-radius: 50%;
        position: fixed;
        right: 50px;
        bottom: 50px;
        overflow: hidden;
        text-align: center;
        text-decoration: none;
        z-index: 50;
        animation: shimmy 1s ;
        animation-direction: alternate;
        &::before{
            content: "\f106";
        }
    }
    @keyframes shimmy {
        100% {
            transform: translate(0, 0);    
        }
        0% {
            transform: translate(0, 100px);
        }
        }
    .fixed{
        display: block;
        
    }
</style>