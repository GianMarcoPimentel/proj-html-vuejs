<script>
export default {
    name:'AppCourses',

    data() {
        return {
            courses: [
                {
                    image: '/images/course-02-480x298.jpg',
                    price:'$40.00',
                    learn:'Learning to Write as a Professional Author',
                    lessons:'20 Lessons',
                    students:'50 Students',
                },
                {
                    image: '/images/stock-full-hd-03-480x298.jpg',
                    price:'Free',
                    learn:'Customer-centric Info-Tech Strategies',
                    lessons:'24 Lessons',
                    students:'769 Students'
                },
                {
                    image: '/images/stock-full-hd-04-480x298.jpg',
                    price:'$19.00',
                    learn:'Open Programming Courses for Everyone: Phytomn',
                    lessons:'17 Lessons',
                    students:'62 Students'
                },
                {
                    image: '/images/stock-full-hd-06-480x298.jpg',
                    price:'$26.00',
                    learn:'Academic Listening and Note-taking',
                    lessons:'14 Lessons',
                    students:'67 Students'
                },
                {
                    image: '/images/course-featured-image-01-480x298.jpg',
                    price:'$39.00',
                    learn:'Master jQuery in a Short Period of Time',
                    lessons:'6 Lessons',
                    students:'51 Students'
                },
                {
                    image: '/images/stock-full-hd-05-480x298.jpg',
                    price:'$59.00',
                    learn:'Introducing to Javascript for Beginners',
                    lessons:'14 Lessons',
                    students:'76 Students'
                },
                
            ]
    }
}
}
</script>

<template >
    <div class="app-cousers">
        
        <div class="container">
            <div id="heading">
                <h6>stimulated to learn?</h6>
                <h3>Featured Online Courses</h3>
    
            </div>
            <div class="choice">
                <div
                v-for="cours in courses"
                id="courses" 
                >
                    <img :src=" cours.image " alt="">
                    <div id="description-cours">
        
                        <div class="price">
                            {{ cours.price }}
                        </div>

                        <div class="learn">
                            {{ cours.learn }}
                        </div>
                        
                        <div id="notions">
                            <div class="lessons">
                                {{ cours.lessons }}
                            </div>
                            <div class="students">
                                {{ cours.students }}
                            </div>
                        </div>
        
                    </div>
                </div>
            </div>
    
            <div id="footer">
                <button> View all courses -</button>
            </div>
        </div>
    </div>
</template>

<style lang="scss">
.app-cousers{
    background-color: #F5F7FA;
}
#heading{

    padding-top: 40px;
    margin-bottom: 30px;
    text-align: center;
    
    h6{
        color: #696969;
        text-transform: uppercase;
    }
    h3{
        color: #3f3a64;
    }
}
.choice{
    display: flex;
    justify-content: center;
    align-content: center;
    flex-flow: row wrap;
    gap: 20px;
}
#courses{
    width: calc(50% - 10px);
    display: flex;
    align-items: center;
    gap: 20px;

    margin-top: 65px;
    img{
        width: 110px;
        height: 110px;
        border-radius: 50%;
        object-fit: cover;
        object-position: center;
    }
    #notions{
        display: flex;
        gap : 30px;

        color: #696969;
    }
}
.price{
    color:#20ad96;
    font-weight: bolder;
}
.learn{
    color: #3f3a64;
    font-weight: bold;
}

#footer{
    text-align: center;

    button{
        background-color: #20ad96;
        color: white;
        padding: 5px 20px;
        border: none;
        border-radius: 4px;

        margin-top: 40px;
    }
}
</style>