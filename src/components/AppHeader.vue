<script>

export default{
    name: 'AppHeader',

    data() {
        return {
            logos: [
                "/images/client-logo-01.png",
                "/images/client-logo-02.png",
                "/images/client-logo-03.png",
                "/images/client-logo-04.png",
                "/images/client-logo-05.png",
                "/images/client-logo-06.png",

            ],
        }
    },
}
</script>
 
<template>
<div class="container">
    <div class="introduction">
        <div class="introduction-text">
            <h1>
                Distant learning for futhure expansion
            </h1>
            <span>
                Learning is a life-lang journey thet in fact we never find the terminate stop. Stop searching, enjoy the process.
            </span>
            <button class="btn">
                <i class="fa-solid fa-download"></i> Download free guide
            </button>
            <div class="question">
             
                    Have question? <span>Get Free Sample <i class="fa-solid fa-arrow-right"></i></span>
               
            </div>
        </div>

        <div class="introduction-image">
            <img class="img-green" src="/public/images/maxcoach-shape-07-100x100.png" alt="">
            <img class="img-gray" src="/public/images/maxcoach-shape-08.png" alt="">
            <img class="img-gray2" src="/public/images/maxcoach-shape-08.png" alt="">
            <img class="img-circle" src="/public/images/maxcoach-shape-02.png" alt="">
            <div class="circle">

            </div>

        </div>
    </div>
</div>
    <div class="container">

        <div class="logos">
            <div 
            v-for="logo in logos"
            class="image">
                <img :src="logo" alt="">
            </div>
        </div>
    </div>

</template>

<style>
.introduction{
    display: flex;
    align-items: center;
    justify-content: space-between;
    .introduction-text{
        width: 320px;
        display: flex;
        flex-flow: column;
        gap: 10px;
    }
    .introduction-text{
        display: flex;
        flex-flow: column;
        gap: 10px;
        h1{
            color: #3f3a64;
            font-weight: bold;
        }
        span{
            color: #696969;
        }
        .btn{
            border: none;
            border-radius: 6px;
            background-color: #20ad96;
            color: white;

            padding: 12px 30px;
            font-weight: bold;

            margin: 10px 0px;
        }
        .question{
            display: flex;
            align-items: center;
            gap: 4px;
            color: #696969;
            span{
                display: flex;
                align-items: center;
                gap:4px;
                color:#20ad96;
                font-weight: bold;
            }
        }
    }
    .introduction-image{
            width: 370px;
            height: 370px;
            border-radius: 50%;

            background-image: url("/public/images/about-me-profile-ohm4dxoearqbxny7q3bq1pzbdgofdx0tobbeqcvzd0.jpg");
            background-size: cover;

            position: relative;
        
            .img-green{
                position: absolute;
                bottom: 0;
                right: 60px;
                z-index: -2;
            }
            
            .img-gray{
                position: absolute;
                top: 50px;
                left: -80px;
                z-index: -2;
            }
            .img-gray2{
                position: absolute;
                top: 150px;
                left: -80px;
                z-index: -2;
            }
            .img-circle{
                width: 80px;
                position: absolute;
                top: 80px;
                right: -80px;
            }
            .circle{
                width: 50px;
                height: 50px;
                border: 5px solid #ECC5AB;
                border-radius: 50%;

                position: absolute;
                bottom: 100px;
                left: -40px;
                z-index: -1;
            }
    }
}
    .logos{
        display: flex;
        align-items: center;
        justify-content: space-between;
    }
</style>