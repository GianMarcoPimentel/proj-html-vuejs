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
            <img src="/public/images/about-me-profile-ohm4dxoearqbxny7q3bq1pzbdgofdx0tobbeqcvzd0.jpg" alt="">
        </div>
    </div>
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
        img{
            width: 370px;
            height: 370px;
            border-radius: 50%;
            object-fit: cover;
    
        }
    }
}
    .logos{
        display: flex;
        align-items: center;
        justify-content: space-between;
    }
</style>