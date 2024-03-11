<script>
export default {
    name:'AppCourses',

    data() {
        return {
            courses: [
                {
                    img: '',
                    price:'',
                    learn:'',
                    lessons:'',
                    students;'',
                },
                {
                    img: '',
                    price:'',
                    learn:'',
                    lessons:'',
                    students;'',
                },
                {
                    img: '',
                    price:'',
                    learn:'',
                    lessons:'',
                    students;'',
                },
                {
                    img: '',
                    price:'',
                    learn:'',
                    lessons:'',
                    students;'',
                },
                {
                    img: '',
                    price:'',
                    learn:'',
                    lessons:'',
                    students;'',
                },
                {
                    img: '',
                    price:'',
                    learn:'',
                    lessons:'',
                    students;'',
                },
                
            ]
    },
}
</script>

<template>
    <div class="container">
        <div id="heading">
            <h6>stimulated to learn?</h6>
            <h3>Featured Online Courses</h3>

        </div>

        <div id="courses">
            <img src="" alt="">
            <div id="description-cours">

                <div class="price"></div>

                <div class="learn"></div>

                <div>
                    <div class="lessons"></div>
                    <div class="students"></div>
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