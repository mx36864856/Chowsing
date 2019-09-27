<template>
    <div class="community">
       <nav-component></nav-component>
        <div class="title">
            <div v-on:click="tab(index)" v-for="(item,index) in title"  :class="{border: curId === index}">{{item.text}}</div>
        </div>
        <div class="title-1 select show" >
            <div class="title-1-top" v-for="(item,index) in cont">
                <span><img :src="item.src"></span>
                <span>{{item.text}}</span>
            </div>
            <div class="title-1-bottom">
                <div class="bottom-1" v-for="(item,index) in bottom">
                    <div :style="{backgroundImage:'url('+ item.src +')'}"></div>
                    <div>
                        <p>{{item.one}}</p>
                        <p>{{item.two}}</p>
                        <p>{{item.three}}</p>
                    </div>
                    <span>{{item.four}}</span>
                </div>
            </div>
        </div>
        <div class="title-2 select">
            <div class="top">
                <span>全部商圈<img src="../assets/箭头.svg"></span>
                <span>智能排序<img src="../assets/箭头.svg"></span>
                <span>筛选<img src="../assets/箭头.svg"></span>
            </div>
                <div class="pic" v-for="(item,index) in bottom_2">
                    <div :style="{backgroundImage:'url('+ item.src +')'}"></div>
                    <div>
                        <p>{{item.one}}</p>
                        <p>{{item.two}}</p>
                    </div>
                    <span>{{item.four}}</span>
                </div>
        </div>
        <Move></Move>
    </div>
</template>

<script>
    import Move from "../components/move";
    import NavComponent from "../components/header-Component";
    import img1 from "../assets/community1/anquan@2x.png";
    import img2 from "../assets/community1/zicha@2x.png";
    import img3 from "../assets/community1/yao@2x.png";
    import img4 from "../assets/community1/zhishi@2x.png";
    import bottom1 from "../assets/community1/u=1083058977,800330093&fm=26&gp=0@2x.png";
    import bottom2 from "../assets/community1/u=306386875,768612393&fm=11&gp=0@2x.png";
    import bottom3 from "../assets/community1/u=2846550785,2572289646&fm=26&gp=0@2x.png";
    import content1 from "../assets/commumity2/u=4148900907,3699594255&fm=26&gp=0@2x.png";
    import content2 from "../assets/commumity2/4@2x.png";
    import content3 from "../assets/commumity2/u=118244653,3245939313&fm=26&gp=0@2x.png";
    import content4 from "../assets/commumity2/u=2019289494,2726267960&fm=26&gp=0@2x.png";

    export default {
        name: "Community",
        components: {
            NavComponent,
            Move
        },
        data(){
            return{
                curId: 0,
                title:[
                    {
                    text:'养宠心得',
                },{
                    text:'萌宠之家'
                }],
                cont:[
                    {
                    src:img1,text:'饮食安全'
                },{
                    src:img2,text:'病症自查'
                },{
                    src:img3,text:'驱虫选药'
                },{
                    src:img4,text:'知识库'
                },],
                bottom:[{
                    src:bottom1,one:'星言家',two:'家庭伦理剧之喵的相处',three:'有时候想给猫咪找个伴',four:'点赞  168'
                },{
                    src:bottom2,one:'萌宠星球',two:'夏日补水小能手',three:'众所周知主食是可以满足主子们...',four:'点赞  145'
                },{
                    src:bottom3,one:'E博士',two:'猫粮该怎么选？看这篇就够了',three:'猫粮该怎么选？看这篇就够了',four:'点赞  233'
                }],
                bottom_2:[{
                    src:content1,one:'宠物小屋',two:'省体育场 宠物店',four:'<100m'
                },{
                    src:content2,one:'宠Ta萌宠生活馆',two:'小雁塔 宠物店',four:'167m'
                },{
                    src:content3,one:'火星宠物',two:'小雁塔 宠物店',four:'237m'
                },{
                    src:content4,one:'宠物小屋',two:'宠物小屋',four:'577m'
                }],
            }
        },
        methods: {
            tab (index) {
                this.curId = index;
                let content = document.querySelectorAll('.select');
                for (let i = 0; i < content.length; i++){
                    content[i].classList.remove('show');
                }
                content[index].classList.add('show')
            }
        }
    }
</script>

<style lang="scss" scoped>
.title{
    margin: 0 .15rem;

    div{
        background-color: #fff;
        float: left;
        width: 1.7rem;
        height: .45rem;
        font-size: .18rem;
        color: #333;
        text-align: center;
        line-height: .45rem;
        position: relative;
        &:nth-child(1){
            border-radius: .1rem 0 0 .1rem;
        }
        &:nth-child(2){
            border-radius: 0 .1rem .1rem 0;
        }
    }
    .border:after{
        content: '';
        display: block;
        position: absolute;
        height: 0;
        width: .46rem;
        bottom: 0;
        left: .6rem;
        border: #ab7246 .01rem solid;
    }
}
.community{
    div:nth-child(2){}
    background-color: black;
}
.title-1{
    .title-1-top{
        width: .55rem;
        height: .5rem;
        float: left;
        margin: .15rem .17rem .3rem .2rem;
        font-size: .13rem;
        text-align: center;
        span{
            display: block;

            &:nth-child(1){
                height: .3rem;
                width: .3rem;
                margin: 0 auto;
                background-color: #AB7246;
                border-radius: .05rem;
                img{
                   height: .14rem;
                    margin-top: .08rem;
                }
            }
        }
    }
    .title-1-bottom{
       float: left;
        padding: 0 .15rem;
        .bottom-1{
            height: .77rem;
            width: 3.25rem;
            background-color: #fff;
            border-radius: .13rem;
            padding: .1rem .1rem;
            margin-bottom: .2rem;
            position: relative;
            span{
                display: block;
                position: absolute;
                right: 0;
                top: .15rem;
                color: #ff8300;
                font-size: .1rem;
                margin-right: .1rem;
            }
            div{
                float: left;
                &:nth-child(1){
                    border-radius: .13rem;
                    height: .77rem;
                    width: .79rem;
                    background: no-repeat center / cover;
                }
                &:nth-child(2){
                    margin-left: .15rem;
                    p:nth-child(1){
                        font-size: .17rem;
                        margin-bottom: .1rem;
                        color: #333;
                    }
                    p:nth-child(2){
                        font-size: .14rem;
                        margin-bottom: .08rem;
                        color: #666;
                    }
                    p:nth-child(3){
                        font-size: .11rem;
                        color: #999;
                    }
                }
            }

        }
    }
}
.title-2{
    width: 100%;
    .top{
        height: .5rem;
        float: left;
        display: flex;
        margin: 0 .15rem;
    span{
        display: block;
        float: left;
        width: .88rem;
        height: .16rem;
        line-height: .5rem;
        font-size: .17rem;
        margin-right: .44rem;
        position: relative;
        img{
            height: .16rem;
        }
    }
    }
    .pic{
        background-color: #fff;
        float: left;
        width: 100%;
        padding: .1rem .18rem .11rem .15rem;
        margin-bottom: .15rem;
        position: relative;
        div{
            float: left;
        }
        div:nth-child(1){
            height: .76rem;
            width: .79rem;
            border-radius: .05rem;
            position: relative;
            background: no-repeat center / cover;
        }
        div:nth-child(2){
            padding-left: .1rem;
            p:nth-child(1){
                padding-top: .17rem;
                font-size: .17rem;
                color: #333;
                padding-bottom: .1rem;
            }
            p:nth-child(2){
                font-size: .12rem;
            }
        }
        span{
            position: absolute;
            bottom: .21rem;
            right: .51rem;
            font-size: .12rem;

        }
    }
}
.community .select{
    display: none;
}
.community .select.show{
        display: block;
    }
</style>