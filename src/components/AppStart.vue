<script>
export default{
    name:'AppStart',

    data(){
        return {
            profiles: [
                {
                    presentation:"It's choice of quality for people with special needs",
                    description:"I'm very strict perosn so I required everything to be organized and neat. Then, I'll be able to make things right and shine. MaxCoach guys just got me.",
                    image:'/images/testimonial-avata-03.jpg',
                    name:'Florence Themes',
                    work:'/ Multimedia Admin',
                },
                {
                    presentation:"High level of efficiency and scientific teaching methods",
                    description:"I am free to learn at my own pace, follow my owm schedule and choose the subject I want to learn from the syllabus. Great study portal for people like me.",
                    image:'/images/testimonial-avata-02.jpg',
                    name:'Mina Hollace',
                    work:'/ Freelancer',
                },
                {
                    presentation:"Profesional ream of specialisrs and passionate mentors at reach",
                    description:"I nedd to get a certification for English profiency and MaxCoach is my best choice. Their tutors are smart and prosfessional when dealing with students",
                    image:'/images/testimonial-avata-04.jpg',
                    name:'Madley Pondor',
                    work:'/ IT Specialist',
                },

            ]
        }
    }
}
</script>

<template>
<div class="appstart">
    <div class="profile-cards">
        <div 
        v-for="profile in profiles"
        class="cards">
            <h2>{{ profile.presentation }}</h2>
            <span>{{ profile.description }}</span>
            <div class="profile">
                <img :src=" profile.image" alt="">
                <div class="profile-user">
                    <h2>{{ profile.name }}</h2>
                    <span>{{ profile.work }}</span>
                </div>
            </div>
        </div>
    </div>
    <div class="container">
        <div class="started-now">
            <div>
                <div class="circle">
    
                </div>
                <img src="/public/images/maxcoach-shape-01.png" alt="">

            </div>
        
            <div class="start">
                <h3>Start today for getting <span>Online Certification</span></h3>
                <h2>You can be your own guiding star with our help</h2>
                <button>
                    Get strated now
                </button>
            </div>
            <div class="img-circle">
                <img  src="/public/images/maxcoach-shape-02.png" alt="">
            </div>
        </div>
    </div>
</div>
</template>

<style>
.appstart{
    background-color: #f8f8f8;
}
.profile-cards{
    display: flex;
    justify-content: space-around;
    align-items: center;
    gap: 30px;
    .cards{
        width: calc(100% / 3 - (30px / 3 * 2));
    }
    .profile{
        display: flex;
        align-content: center;
        gap: 20px;

        img{
            width: 80px;
            height: 80px;
            border-radius: 50%;
        }
        .profile-user{
            display: flex;
            flex-flow: column;
            gap: 10px;
        }
    }
}
.started-now{
    display: flex;
    justify-content: space-between;
    align-items: center;
    .circle{
        width: 50px;
        height: 50px;
        border: 5px solid #E6DCD2;
        border-radius: 50%;
    }
    .start{
        display: flex;
        flex-flow: column;
        align-items: center;
        gap: 10px;

        color: #3f3a64;
        font-weight: bold;

        span{ 
            color: #20ad96;
            font-weight: normal;
        }
        button{
            border: none;
            border-radius: 6px;
            background-color: #20ad96;
            color:white;
            font-weight: bold;
            padding: 12px 50px;
        }

    }
}
.img-circle{
    width: 80px;
    position: relative;

    img{
        width: 100%;
        position: absolute;
        top: 0;
        right: 0;
    }
}
</style>