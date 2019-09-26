<template>
    <div class="header">
    <div>猫咪V</div>
    <div>
        <img src="../assets/搜索.svg" alt=""><input type="text" placeholder="请输入搜索内容"></div>
    <img src="../assets/提醒.svg" alt="">
    </div>
</template>

<script>
    export default {
        name: "header-Component"
    }
</script>

<style lang="scss" scoped>
.header{
    width: 100%;
    height: .3rem;
    padding: .1rem 0 .1rem;
    background-color: #f7f5ef;
    div{
        float: left;
        &:nth-child(1){
            padding: 0 .1rem;
            height: .3rem;
            font-size: .18rem;
            font-weight:bold;
            color:rgba(51,51,51,1);
            line-height:0.3rem;

        }
        &:nth-child(2){
         position: relative;
            img{
                height: .2rem;
                position: absolute;
                top: .05rem;
                z-index: 2;
            }
            input{
                width:2.3rem;
                height:0.3rem;
                background:rgba(255,255,255,1);
                padding-left: .26rem;
                position: absolute;
                border: 0 solid;
                border-radius: .05rem;
                outline: none;
                font-size: .12rem;
            }
        }
    }
    img{
        float: right;
        height: .31rem;
        width: .31rem;
        margin-right: .12rem;
    }
}
</style>