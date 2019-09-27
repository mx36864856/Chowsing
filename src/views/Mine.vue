<template>
    <div class="mine">
       <div class="header">
           <img src="../assets/提醒.svg">
           <div class="header-picture">
               <div><img src="../assets/mine/21@2x.png"></div>
               <div>
               <p>Leago</p>
               <p>宠幸号：saida</p>
               </div>
           </div>
       </div>
        <div class="content">
            <div v-for="item in content" class="title">
                <img :src="item.href">
                <span>{{item.text}}</span>
                <img src="../assets/mine/)@2x.png">
            </div>
        </div>
        <Move></Move>
    </div>
</template>

<script>
    import Move from "../components/move";
    import img1 from '../assets/mine/7@2x.png'
    import img2 from '../assets/mine/5@2x.png'
    import img3 from '../assets/mine/3@2x.png'
    import img4 from '../assets/mine/6@2x.png'
    import img5 from '../assets/mine/1@2x.png'
    import img6 from '../assets/mine/4@2x.png'
    export default {
        name: "Mine",components: {
            Move
        },
        data(){
            return{
                content:[{
                    href:img1,text:'我的萌宠'
                },{
                    href:img2,text:'我的订单'
                },{
                    href:img3,text:'我的钱包'
                },{
                    href:img4,text:'我的收藏'
                },{
                    href:img5,text:'我的服务'
                },{
                    href:img6,text:'设置'
                }]
            }
        }
    }

</script>

<style lang="scss" scoped>
.mine{
    background-color: #f7f5ef;
    .header{
        width: 100%;
        height: 1.2rem;
        padding-top: .1rem;
        >img{
            height: .28rem;
            float: right;
            margin-right: .14rem;
        }
        .header-picture{
            margin-left: .15rem;
            div:nth-child(1){
                float: left;
                width: .68rem;
                height: .68rem;
                img{
                    height: .68rem;
                }
            }
            div:nth-child(2){
                float: left;
                font-size: .18rem;
                margin-top: .28rem;
                font-weight: 400;
                padding-left: .1rem;
                p:nth-child(2){
                    font-size: .14rem;
                    margin-top: .1rem;
                }
            }
        }
    }
    .content{
        .title{

            height: .51rem;
            font-size: .17rem;
            background-color: #fff;
            margin-bottom: .2rem;
            padding-left: .17rem;
            img:nth-child(1){
                height: .24rem;
                margin: .14rem .2rem 0 0;
                float: left;
            }
            span{
                float: left;
                margin-top: .14rem;
            }
            img:nth-child(3){
                float: right;
                margin-top: .22rem;
                height: .09rem;
                margin-right: .2rem;
            }
        }
    }
}    
</style>