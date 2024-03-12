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
            <h2>Smart tutoring </h2>
            <h2>Program For Benefits</h2>
        </div>

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

        <div class="container">
            <div class="videotutorial">

                <div class="video">
                    <img class="video-image" src="/public/images/home-2-popup-video-poster.jpg" alt="">
                    <img class="video-icon" src="/public/images/icon-youtube-play.png" alt="">
                </div>
                <div class="text">
                    <div class="companionship">
                        <span>GET STARTED EFFORTLESSLY</span>
                        <h1>Enjoy Our <span>Companionship</span></h1>
                        <span>Sneek peek into what has in store fot you on our online teaching and mentoring portal. Seek for some hidden hints og early-bird rewards as well.</span>
                    </div>
                    <div class="download">
                        Download free guidebook <i class="fa-solid fa-arrow-right"></i>
                    </div>
                </div>

            </div>
        </div>

    </div>
</template>

<style lang="scss">
h3{
    text-align: center;
}
.title-tutoring{
    display:flex ;
    justify-content: center;
    gap:4px;
}
.tutoring{
    display: flex;
    justify-content: space-between;

    .hookup{
        display: flex;
        align-items: center;
        gap: 8px;

        color: #3f3a64;

        font-weight: bold;
    } 
}
.videotutorial{
    display: flex;
    justify-content: space-between;
    align-items: center;
    .video{
        width: 400px;
        height: 100%;
        position: relative;
    
        .video-image{
            width: 100%;
        }
        .video-icon{
            width: 80px;
            position:absolute;
            top:50%;
            left: 50%;
        }
    }
    .text{
        width: 260px;
    }
}
</style>