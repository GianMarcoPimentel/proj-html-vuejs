<script>

export default{
    name:'AppTutoring',

    data() {
        return {
            programs:[
                {
                    image:'/images/home-2-image-box-01.png',
                    activity:'Costumize Preferences',
                    description:'Learners are given the right to arrange and costumize their study schedule and timetable based an preferences',
                    hookup:'Start here'
                },
                {
                    image:'/images/about-us-02-image-box-02.png',
                    activity:'Cloud Storage',
                    description:'You can store online lessons via online cloud or download to your device and revise lessons on the way',
                    hookup:'Get Free Quote',
                },{
                    image:'/images/home-2-image-box-03.png',
                    activity:'Multimedia Channels ',
                    description:'We provide study materilas with various formats video, audio, slides, doc, prints, books and applications.',
                    hookup:'Start now',
                },

            ]
        }
    },
}
</script>

<template>
    <div class="container">

        <h3> maxcoach available courses</h3>

        <div class="title-tutoring">
            <h2>Acces</h2>
            <h2 class="green">Smart tutoring </h2>
            <h2>Program For Benefits</h2>
        </div>
    </div>
    <div class="container">

        <div class="tutoring">

            <div 
            v-for="program in programs"
            class="cards">
                <img :src="program.image" alt="">
                <div class="activity">
                    {{ program.activity }}
                </div>
                <div class="description">
                    {{ program.description }}
                </div>
                <div class="hookup">
                    {{ program.hookup }} <i class="fa-solid fa-arrow-right"></i>
                </div>
            </div>
            
        </div>
    </div>

        <div class="container">
            <div class="videotutorial">

                <div class="video">
                    <!-- <img class="video-image" src="/public/images/home-2-popup-video-poster.jpg" alt=""> -->
                    <img class="video-icon" src="/public/images/icon-youtube-play.png" alt="">
                    <!-- <img class="cloud" src="/public/images/cloud.svg" alt=""> -->
                    <svg xmlns="http://www.w3.org/2000/svg" version="1.1" width="200px" height="202px" viewBox="0 0 200 202">
                        <path class="elementor-shape-fill cloud" d="M139.374493,198.087515 C155.702187,206.99353 190.724846,197.001323 197.677982,159.049528 C204.827153,120.027728 184.496324,118.997566 188.045232,104.801934 C202.287755,83.6528313 204.827153,56.662651 190.073179,40.4146034 C153.570125,2.39058926 144.444362,48.0194062 114.025151,20.1351292 C101.727304,7.83728238 83.0989526,-6.73517414 56.2286492,3.40456297 C18.2385839,17.7404371 27.3303985,47.659333 27.3303985,69.3128542 C27.3303985,76.9370868 3.11408002,91.2696589 0.460095291,110.885776 C-2.88628833,135.619549 12.6277797,168.175291 27.3303985,179.329002 C50.6517938,205.692318 86.6478605,199.608476 102.87144,190.482713 C116.802125,182.646702 128.220783,192.003673 139.374493,198.087515 Z"></path>
                    </svg>  

                    <img class="img-05" src="/public/images/maxcoach-shape-05-100x100.png" alt="">
                    <img class="img-07" src="/public/images/maxcoach-shape-07-100x100.png" alt="">
                </div>
                <div class="text">
                    <div class="companionship">
                        <span>GET STARTED <span class="blue">EFFORTLESSLY</span> </span>
                        <h1 class="blue">Enjoy Our <span class="green">Companionship</span></h1>
                        <span>Sneek peek into what has in store fot you on our online teaching and mentoring portal. Seek for some hidden hints og early-bird rewards as well.</span>
                    </div>
                    <div class="green download">
                        Download free guidebook <i class="fa-solid fa-arrow-right"></i>
                    </div>
                </div>

            </div>
        </div>

    
</template>

<style lang="scss">
h3{
    text-align: center;
    text-transform: uppercase;
    font-size: 10px;
    color: #696969;
}
.title-tutoring{
    display:flex ;
    justify-content: center;
    gap:4px;
    color: #3f3a64;
    font-weight: bold;
    .green{
        color: #20ad96;
        font-weight: normal;
    }
}
.tutoring{
    display: flex;
    justify-content: space-between;
    gap: 20px;
    
    .cards{
        display: flex;
        flex-flow: column;
        align-items: start;
        justify-content: space-between;
        gap: 10px;
        
        .activity{
            color: #3f3a64;
            font-weight: bold;
        }

        .description{
            color: #696969;
        }
        .hookup{
            display: flex;
            align-items: center; 
            gap: 8px;
    
            color: #3f3a64;
            opacity: 0.7;
    
            font-weight: bold;
    
            margin-top: 40px;
        } 
    }

}
.videotutorial{
    display: flex;
    justify-content: space-between;
    align-items: center;
    .video{
        width: 450px;
        height: 300px;
        background-image: url("/public/images/home-2-popup-video-poster.jpg");
        background-size: cover;
        border-radius: 8px;
        position: relative;
        
        .video-icon{
            width: 80px;
            position:absolute;
            top:40%;
            left: 40%;
        }
        svg{
            width: 100px;
            position: absolute;
            top: -100px;
            left: -40px;
            fill: #E5C791;
            z-index: -2;
        }
        .img-05{
            position: absolute;
            top: 40px;
            left: -60px;
            z-index: -1;
        }
        .img-07{
            position: absolute;
            bottom: -60px;
            right: -10px;
            z-index: -1;
        }
    }
    .text{
        width: 260px;
        color: #696969;
        padding: 10px;
    .companionship{
        display: flex;
        flex-flow: column;
        gap: 10px;
    }
    .blue{
        color: #3f3a64;
    }
    .green{
        color: #20ad96;
        font-weight: normal;
    }
    .download{
        font-weight: bold;
        margin-top: 20px;
    }
    
    }
}

</style>