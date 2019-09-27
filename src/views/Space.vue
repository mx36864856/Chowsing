<template>
    <div class="space">
        <div class="catalogue-top"><a href="/classify"><img src="../assets/catalogue/(@2x.png"></a>我的订单</div>
        <div class="content">
            <div></div>
            <div>啊哦~小主子你还没有订单哦~</div>
            <div><button>点击添加</button></div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "Space"
    }
</script>

<style lang="scss" scoped>
    .catalogue-top{
        width: 100%;
        height: .5rem;
        text-align: center;
        font-size: .17rem;
        border-bottom:#BFA77A .01rem solid ;
        position: relative;
        line-height: .5rem;
        img{
            width: .17rem;
           position: absolute;
            left: .14rem;
            top: .14rem;
        }
    }
    .content{
        width: 100%;
        margin-top: 1rem;
        div:nth-child(1){
            height: 2rem;
            width: 1.6rem;
            background: url("../assets/cat@2x.png") no-repeat center / cover;
            margin: 0 auto;
        }
        div:nth-child(2){
            text-align: center;
            font-size: .17rem;
            color: #333;
            margin-top: .67rem;
        }
        div:nth-child(3){
            height: .39rem;
            width: 1.13rem;
            margin: 0 auto;
            margin-top: .46rem;
            button{
                height: .39rem;
                width: 1.13rem;
                background-color: #AB7246;
                color: white;
                font-size: .17rem;
                line-height: .39rem;
                text-align: center;
                border: none;
                border-radius: .05rem;

            }
        }
    }
</style>