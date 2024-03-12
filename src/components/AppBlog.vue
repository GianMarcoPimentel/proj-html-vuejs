<script >

export default {
  name:'AppBlog',

  data() {
    return {
        cards:[
            {
                image:'/images/artist-blog-03-480x352.jpeg',
                type:'artist',
                work:'Brush Stroke Energize Trees in Paintings',
                date:'MAY, 15 2020',
                views:'688 views',
            },
            {
                image:'/images/artist-blog-01-480x352.jpg',
                type:'artist',
                work:'Pocket-Sized Notebooks Hold Miniature Paintings',
                date:'MAY, 15 2020',
                views:'603 views',
            },
        ]
    }
  },

}
</script>

<template>
    <div class="appblog">

        <div class="container">
            <div class="blogs">
                <h4>enjoyable insights</h4>
                <div class="title-blog">
                    <span class="bold">Most Viewed</span>
                    <span>Best Blogs</span>
                </div>
                <ul>
                    <li><i class="fa-solid fa-arrow-right"></i> <span>Became a better blogger: Cntentr Planning</span> </li>
                    <li><i class="fa-solid fa-arrow-right"></i>  <span>Promoting Your Online Business on Pinterest</span> </li>
                    <li><i class="fa-solid fa-arrow-right"></i>  <span>Gamificatione and Game-Based Learning</span> </li>
                    <li><i class="fa-solid fa-arrow-right"></i>  <span>Designing an Online Course from Expert's Perspective</span> </li>
                    <li><i class="fa-solid fa-arrow-right"></i>  <span>Why Online Courses Are the Future of Education</span> </li>
                </ul>
            </div>
            <div 
            v-for="card in cards"
            class="card">
                <img :src="card.image" alt="">
                <div class="description">
                    <small>{{ card.type }}</small>
                    <small>{{ card.work }}</small>
                    <div class="footer-card">
                        <div class="date">
                            <i class="fa-regular fa-calendar"></i> <small>{{ card.date }}</small>
                        </div>
                        <div class="views">
                            <i class="fa-regular fa-calendar"></i> <small>{{ card.views }}</small>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

</template>

<style lang="scss" scoped>
.appblog{
    background-color: #F5F1ED; 
   
}
.container{
    display: flex;
    gap: 30px;

    .title-blog{
        display: flex;
        gap: 10px;
        color: #20ad96;
        font-size: 20px;
        
        .bold{
            color: #3f3a64;
            font-weight: bold;
        }
    }
    ul{
        list-style-type: none;

        li{
            line-height: 2em;
            display: flex;
            
            gap: 10px;

            color:#3f3a64;

            font-weight: bold;
        }
    }
    
}
.card{
    display: flex;
    flex-flow: column;
    width: 300px;
    background-color: white;
    border-radius: 8px;
    img{
        width: 100%;
        border-top-right-radius: 8px;
        border-top-left-radius: 8px;
        
    }
    .description{
        display: flex;
        flex-flow: column;
        justify-content: space-between;
        padding: 10px;
    }
    .footer-card{
        color: #696969;

        display: flex;
        gap: 20px;

        .date{
            display:flex ;
            align-items: center;
            gap : 4px;
        }
        .views{
            display: flex;
            align-items: center;
            gap: 4px;
        }
    }
}
</style>
