<script>
export default{
    name:'AppStart',

    data(){
        return {
            activeProfileIndex : '',

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
    },
    methods : {
        pointClick(){
            this.activeProfileIndex == 0;
            const profile = document.getElementById('cards');
            profile.style.opacity = 1;
        },
        pointClick2(){
            this.activeProfileIndex == 1;
            const profile = document.getElementById('cards');
            profile.style.opacity = 1;
        },
        pointClick3(){
            this.activeProfileIndex == 2;
            const profile = document.getElementById('cards');
            profile.style.opacity = 1;
        }
        
    }

}

</script>

<template>
<div class="appstart">
    <div class="profile-cards">
        <div 
        v-for="(profile,index) in profiles"
        
        id="cards"
        style="opacity : 0.7">
        
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
    <div class="icon">
            <i @click="pointClick()" class="fa-solid fa-circle"></i>
            <i @click="pointClick2()" class="fa-solid fa-circle"></i>
            <i @click="pointClick3()" class="fa-solid fa-circle"></i>
            <i class="fa-solid fa-circle"></i>
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
    padding: 30px ;
    margin-top: 30px;
}
.profile-cards{
    
    display: flex;
    justify-content: space-around;
    align-items: center;
    gap: 30px;
    h2{
        color: #3f3a64;
    }
    span{
        color: #696969;
    }
    #cards{
        width: calc(100% / 3 - (30px / 3 * 2));
        height: 100%;
        
       
        border-radius: 10px;
        display: flex ;
        flex-flow: column;
        
        gap: 20px;

        padding: 20px;
        background-color: white;
    }
    
    .profile{
       
        display: flex;
        align-items: start;
        gap: 20px;

        padding: 20px;
        img{
            width: 60px;
            height: 60px;
            border-radius: 50%;
        }
        .profile-user{
            display: flex;
            flex-flow: column;
            gap: 10px;

            font-size: 10px;
        }
    }
}
.icon{
    padding: 20px 0px;
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 10px;
   
    i{
        color: #3f3a64;
    opacity: 0.6;
    }


}
i:hover{
    opacity: 1;
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