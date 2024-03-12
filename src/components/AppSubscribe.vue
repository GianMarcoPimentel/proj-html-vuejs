<script>


export default {
  nam:'AppSubscribe'

}
</script>

<template>
<div class="container">
    <div class="appsubscribe">
        <div class="title">
            <span class="bold">Subscribe</span>
            <span>Newsletters </span>
        </div>
        <p>Enter your email address to register to our newsletter subscription delivered on a regular basis!</p>
        <input type="text" placeholder="Enter your email">

    </div>
   
</div>
</template>

<style >
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
 