<template>
    <div class="classify">
        <div class="header">
            <div>猫咪V</div>
            <div>
                <img src="../assets/搜索.svg" alt=""><input type="text" placeholder="请输入搜索内容">
            </div>
            <a href="/space"><img src="../assets/购物车.svg" alt=""></a>
            <img src="../assets/提醒.svg" alt="">
        </div>
        <div class="classify-top">
            <div class="select">分类</div>
            <div>品牌</div>
        </div>
        <div class="content">
            <div class="content-1">
                <p v-on:click="tab(index)" :class="{border: index === curId}" v-for="(item,index) in test" >{{item.text}}</p>
            </div>
            <div v-show="index===curId" v-for="(item, index) in test">
                <p>{{item.text}}</p>
                <div v-for="(item,index) in content">
                    <img :src="item.url">
                    <p>{{item.text}}</p>
                </div>
            </div>
        </div>
        <Move></Move>
    </div>
</template>

<script>
    import Move from "../components/move";
    import NavComponent from "../components/header-Component";
    import img from "../assets/classify/u=2614015722,3752731499&fm=26&gp=0@2x.png";
    export default {
        name: "Classify",
        components: {
            NavComponent,
            Move
        },
        data(){
            return{
                curId: 0,
                test:[
                    {
                    text:'为你推荐'
                },{
                    text:'精选国际'
                },{
                    text:'猫咪洗浴'
                },{
                    text:'消暑补水'
                },{
                    text:'猫咪主粮'
                },{
                    text:'猫咪零食'
                },{
                    text:'猫咪美容'
                },{
                    text:'猫咪玩具'
                },{
                    text:'猫咪保健'
                },{
                    text:'猫咪护理'
                },],
                content:[{
                    url:img,text:'进口猫粮'
                },{
                    url:img,text:'进口猫粮'
                },{
                    url:img,text:'进口猫粮'
                },{
                    url:img,text:'进口猫粮'
                },{
                    url:img,text:'进口猫粮'
                },{
                    url:img,text:'进口猫粮'
                },],

            }
        },
        methods: {
            tab (index) {
                this.curId = index;
            }
        }
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
                    width:2rem;
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
        a{
            img{
            float: right;
            height: .18rem;
            /*width: .31rem;*/
            margin-right: .13rem;
            margin-top: .07rem;
            }
        }
        img:nth-child(4){
            float: right;
            height: .2rem;
            margin-right: .2rem;
            margin-top: .05rem;
        }
    }
.classify-top{
    height: .38rem;
    width: 100%;
    /*margin: 0 .18rem;*/
    div{
        width: 1.65rem;
        height: .26rem;
        background-color: #fff;
        color: #ab7246;
        float: left;
        text-align: center;
        font-size: .14rem;
        margin-top: .12rem;
        line-height: .26rem;
    }
    div:nth-child(1){
        margin-right: .1rem;
        margin-left: .18rem;
    }
    div.select{
        height: .38rem;
        line-height: .38rem;
        background-color: #ab7246;
        color:white;
        border-radius: .05rem .05rem 0 0;
        margin-top: 0;
    }
}
.content{
    div{
        width: 2.5rem;
        float: right;
        p:nth-child(1){
            color: #d3a37e;
            font-size: .17rem;
            line-height: .5rem;
        }
        div{
            width: .83rem;
            height: 1.2rem;
            float: left;
            text-align: center;
            /*margin-right: .05rem;*/
            img{
                height: .72rem;
                width: .72rem;
                margin-bottom: .05rem;
            }
            p{
                font-size: .15rem;
            }
        }
    }
    div.content-1{
        width: 1.2rem;
        float: left;
        p{
            height: .5rem;
            width: 100%;
            background-color: #d3a37e;
            color: #fff;
            font-size: .15rem;
            text-align: center;
            line-height: .5rem;
            position: relative;
        }
        p.border{
            background-color: #fff;
            color: #6a3906;
        }
        .border:after{
            height: .46rem;
            content: '';
            position: absolute;
            left: 0;
            top: .02rem;
            display: block;
            border: #6a3906 .02rem solid;
        }
    }
}
</style>