<template>
    <div class="move">
        <a :href=item.href v-for="item in text">
            <span :style="{backgroundImage: 'url(' +item.src + ')'}"></span>
            <span>{{item.test}}</span>
        </a>
    </div>
</template>

<script>
    import src1 from "../assets/table/jingxuan(1)@2x.png"
    import src2 from "../assets/table/fenlei(1)@2x.png"
    import src3 from "../assets/table/shequ(1)@2x.png"
    import src4 from "../assets/table/wode(1)@2x.png"
    export default {
        name: "sousuo",
        data(){
            return{
                text:[{
                    src:src1,test:'精选',href:'/home'
                },{
                    src:src2,test:'社区',href:'/community'
                },{
                    src:src3,test:'分类',href:'/classify'
                },{
                    src:src4,test:'我的',href:'/mine'
                }],
            }
        }
    }
</script>

<style lang="scss" scoped>
.move{
    position: fixed;
    bottom: 0;
    width: 100%;
    height: .5rem;
    background-color: #fff;
    /*padding-left: .35rem;*/
    a{
        float: left;
        height: .5rem;
        width: .9rem;
        text-decoration: none;
        color: #AB7246;
        font-size: .1rem;
        text-align: center;
        padding-top: .1rem;
        span:nth-child(1){
            display: block;
            width: .18rem;
            height: .19rem;
            background: no-repeat center / cover;
            margin: 0 auto;
        }
    }
}
</style>