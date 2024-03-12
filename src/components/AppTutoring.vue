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
</style>