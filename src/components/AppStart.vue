<script>
export default{
    name:'AppStart',

}
</script>

<template>
<div class="appstart">

    
    <div class="container">
        <div class="started-now">
            <div>
                <div class="circle">
    
                </div>
                <img src="/public/images/maxcoach-shape-01.png" alt="">

            </div>
        
            <div class="start">
                <h3>Start today for getting <span>Online Certification</span></h3>
                <h2>You can be your own guiding star with our help</h2>
                <button>
                    Get strated now
                </button>
            </div>
            <div>
                <img src="/public/images/maxcoach-shape-02.png" alt="">
            </div>
        </div>
    </div>
</div>
</template>

<style>
.appstart{
    background-color: #f8f8f8;
}
.started-now{
    display: flex;
    justify-content: space-between;
    align-items: center;
    .circle{
        width: 50px;
        height: 50px;
        border: 5px solid #E6DCD2;
        border-radius: 50%;
    }
    .start{
        display: flex;
        flex-flow: column;
        align-items: center;
        gap: 10px;

        color: #3f3a64;
        font-weight: bold;

        span{
            color: #20ad96;
            font-weight: normal;
        }
        button{
            border: none;
            border-radius: 6px;
            background-color: #20ad96;
            color:white;
            font-weight: bold;
            padding: 12px 50px;
        }

    }
}
</style>