<script>
export default {
    name:'AppFooter',
    data() {
        return {

            linkLists:[
                {
                    title:'Explore',
                    links:['Start here', 'Blog', 'About us',],
                },
                {
                    title:' ',
                    links:['Start here', 'Blog', 'About us',],
                },
                {
                    title:'Information',
                    links:['Membership', 'Purchase guide', 'Privacy police', 'Terms of services'],
                },
                
                    ]
        }
    },
  }

</script>

<template>
    
  <div class="container">
    <div class="footer">
        <div class="address">
            <h4>Address</h4>
            <ul>
                <li>382 NE 191st St # 87394 Miami, FL 33179-3899</li>
                <li>+1 (305) 547-9909 (9am - 5pm EST,Monday - Friday)</li>
                <li>support@maxcoach.com</li>
            </ul>
            <div class="socials">
                <i class="fa-brands fa-square-facebook"></i>
                <i class="fa-brands fa-twitter"></i>
                <i class="fa-brands fa-instagram"></i>
                <i class="fa-brands fa-linkedin"></i>
            </div>
        </div>
        <div 
        v-for="linkList in linkLists"
        class="lists">
        <h4> {{ linkList.title }} </h4>
        <ul>
            <li
            v-for="link in linkList.links"
            >
            {{ link }}
            </li>
        </ul>
        </div>
    </div>
    <div class="credits">
        © MaxCoach, All Rights Reserved
    </div>

  </div>
</template>

<style >
.footer{
    display: flex;
    justify-content: space-between;
    .address {
        display: flex;
        flex-flow: column;
        align-items: flex-start;
        gap: 10px;

        .socials{
            display: flex;
            gap: 30px;

            color: #696969;
            i{
                font-size: 20px;
                margin-top: 20px;
            }
        }
    }
    
    ul{
        list-style-type: none;
    }
    
    h4{
        color: #3f3a64;
    }

    li{
        color: #696969;
    }

}
.credits{
    width: 50%;
    margin-left: auto;
    margin-right: auto;

    padding-top: 10px;
    text-align: center;
    color: #696969;
}
</style>