<template>
    <div>
         <div class="carousel" :class="small? 'small' : ''">
            <div class="arrow">&#8249;</div>
            <div class="wrapper">
                <img src="../assets/img/spring_printed_dress-400x520.jpg" alt="">
            </div>
            <div class="wrapper">
                <img src="../assets/img/modern_love_tee-400x520.jpg" alt="">
            </div>
            <div class="wrapper">
                <img src="../assets/img/black_leather_jacket-400x520.jpg" alt="">
            </div>
            <div class="wrapper">
                <img src="../assets/img/black_elegant_leather_jacket-400x520.jpg" alt="">
            </div>
             <div class="wrapper">
                <img src="../assets/img/hipster_black_top-400x520.jpg" alt="">
            </div>
            <div class="arrow">&#8250;</div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Carousel',
    props: {
        small: Boolean,
    }
}

</script>


<style scoped lang="scss">
     .small {
        width: 70%;
        margin: auto;  
    }
     .carousel { 
        align-items: center;
        margin-bottom: 60px;
        min-width: 1100px;
        display: flex;
        .wrapper {
            width: calc((100% / 4) - 40px);
            img {
                width: 100%
            }
        }
        .arrow {
            height: 40px;
            width: 20px;
            text-align: center;
            line-height: 40px;
            background: grey;
            color: white;
            flex-shrink: 0;
        }
    }
</style>