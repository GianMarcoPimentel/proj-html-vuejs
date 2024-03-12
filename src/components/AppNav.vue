<script >

export default {
    name:'AppNav',

    data(){
        return {
            links: [
                'Home',
                'Pages',
                'Courses',
                'Features',
                'Blog',
                'Shop',
               

            ]
        }
    }
}
</script>

<template>
    <!-- Imposto la Navbar con 
        - il logo, 
        - i links, e il campo di ricerca 
    -->
<div class="container">

        <nav>
            <div class="logo">
                <img src="/public/images/dark-logo.png" alt="">
            </div>
        
            <div class="links">
        
                <ul>
                <li v-for="link in links">
                    {{ link }} <i class="fa-solid fa-chevron-down"></i>
                </li>
                </ul>
                
                <i class="fa-regular fa-circle-user"></i>

                <input type="text" placeholder="Search" >
                <button><i class="fa-solid fa-magnifying-glass"></i></button>
        
            </div>
        </nav>

</div>

</template>

<style lang="scss"> 
/* Stilizzo:
    - nav
    - links ( ul , li , input)
    
*/
nav{
    display: flex;
    justify-content: space-between;
    align-items: center;

    color: #696969;

    .logo{
        height: 20px;
        display: flex;

        color: #3f3a64;
        .logo-bold{
            font-weight: bold;
        }
    }
    
    .links{
        display: flex;
        align-items: center;
        gap: 10px;

        ul {
            list-style-type: none;
            display: flex;
            gap: 10px;
    
            li{
                color: #696969;
            }
        } 
    }
}
</style>
