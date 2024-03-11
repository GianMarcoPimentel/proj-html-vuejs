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
                    image: '/images/course-02-480x298.jpg',
                    price:'Free',
                    learn:'Customer-centric Info-Tech Strategies',
                    lessons:'24 Lessons',
                    students:'769 Students'
                },
                {
                    image: '/images/course-02-480x298.jpg',
                    price:'$19.00',
                    learn:'Open Programming Courses for Everyone: Phytomn',
                    lessons:'17 Lessons',
                    students:'62 Students'
                },
                {
                    image: '/images/course-02-480x298.jpg',
                    price:'$26.00',
                    learn:'Academic Listening and Note-taking',
                    lessons:'14 Lessons',
                    students:'67 Students'
                },
                {
                    image: '/images/course-02-480x298.jpg',
                    price:'$39.00',
                    learn:'Master jQuery in a Short Period of Time',
                    lessons:'6 Lessons',
                    students:'51 Students'
                },
                {
                    image: '/images/course-02-480x298.jpg',
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

<template>
    <div class="container">
        <div id="heading">
            <h6>stimulated to learn?</h6>
            <h3>Featured Online Courses</h3>

        </div>

        <div
        v-for="cours in courses"
        id="courses" 
        >
            <img :src=" cours.image " alt="">
            <div id="description-cours">

                <div class="price">
                    {{ cours.price }}
                </div>

                <div class="learn"></div>
                    {{  }}
                <div>
                    <div class="lessons">
                        
                    </div>
                    <div class="students">

                    </div>
                </div>

            </div>
        </div>

        <div id="footer">
            <button> View all courses -</button>
        </div>
    </div>
</template>

<style lang="scss">
#heading{
    text-align: center;
    
    h6{
        
        text-transform: uppercase;
    }
}
#courses{
    display: flex;

}
img{
    width: 100px;
    height: 100px;
    border-radius: 50%;
    object-fit: cover;
    object-position: center;
}
#footer{
    text-align: center;

    button{
        background-color: #20ad96;
        color: white;
        padding: 5px 20px;
        border: none;
        border-radius: 4px;
    }
}
</style>