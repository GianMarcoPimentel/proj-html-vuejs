<script>


export default {
  nam:'AppSubscribe'

}
</script>

<template>
<div class="container relative">
    <div class="circle">

    </div>
    <div class="appsubscribe">
        <div class="title">
            <span class="bold">Subscribe</span>
            <span>Newsletters </span>
        </div>
        <p>Enter your email address to register to our newsletter subscription delivered on a regular basis!</p>
        <input type="text" placeholder="Enter your email">

    </div>
    <div class="image">
        <img src="/public/images/maxcoach-shape-02.png" alt="">
    </div>
   
</div>
</template>

<style >
.relative{
    position: relative;
    .image{ 
        width: 80px;
        position: absolute;
        top:100px;
        right: -40px;
    }
    .circle{
        width: 50px;
        height: 50px;
        border: 5px solid #8FD6CA;
        border-radius: 50%;

        position: absolute;
        top: 100px;
        left: -40px;
       
            }
}
.appsubscribe{
    width: 50%;
    margin-right: auto;
    margin-left: auto;

    display: flex;
    flex-flow: column;
    gap: 20px;
}
.title{
    display: flex;
    justify-content: center;
    gap: 10px;

    font-size: 15px;
    color: #20ad96;
    .bold{
        color: #3f3a64;
        font-weight: bold;
    }
}
p{
    text-align: center;
}

</style>
 