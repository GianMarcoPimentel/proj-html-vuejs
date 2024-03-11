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
            
            <span class="logo-bold">Max</span>
            <span>Coach</span>

            </div>
        
            <div class="links">
        
                <ul>
                <li v-for="link in links">
                    {{ link }}
                </li>
                </ul>
        
                <input type="text" placeholder="Search">
        
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

    padding: 10px 0px;
    color: #696969;

    .logo{
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
