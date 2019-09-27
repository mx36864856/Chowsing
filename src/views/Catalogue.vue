<template>
    <div class="catalogue">
        <div class="err">
        </div>
        <div class="catalogue-top"><img src="../assets/catalogue/(@2x.png"></div>
        <div class="catalogue-bottom">
            <div class="text">
                <div><input class="input1" type="text" placeholder="请输入用户名/手机号"> <img src="../assets/catalogue/我(2)@2x.png"></div>
                <div><input class="input2" type="password" placeholder="请输入密码"> <img src="../assets/catalogue/密码(3)@2x.png"></div>
                <div>忘记密码</div>
                <div><button v-on:click="userName">登录</button></div>
                <div>注册</div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "Catalogue",
        methods: {
            userName () {
                let input1 = document.querySelector('.input1').value;
                let input2 = document.querySelector('.input2').value;
                let err = document.querySelector('.err');
                console.log(!/^[A-Za-z0-9]+$/.test(input1));

                if (!/^[A-Za-z0-9]+$/.test(input1)){
                   err.classList.add('show');
                   err.innerHTML = '用户名为数字和字母';
                   setTimeout(function () {
                       err.classList.remove('show')
                   },2000)
                }else{
                    if (!/^[A-Za-z0-9]+$/.test(input2)){
                        err.classList.add('show');
                        err.innerHTML = '密码为数字和字母';
                        setTimeout(function () {
                            err.classList.remove('show')
                        },2000)
                    }else {
                        window.location.href = "/home"
                    }
                }
            }
        }
    }

</script>

<style lang="scss" scoped>
    .catalogue{
        position: relative;
    }
.err{
    position: fixed;
    top: 0;
    width: 100%;
    height: 0;
    z-index: 3;
    overflow: hidden;
    background-color: rgba(1,1,1,.4);
    color: white;
    transition: .2s;
    line-height: .5rem;
    text-align: center;
    font-size: .18rem;
}
.err.show{
    height: .5rem;
}
.catalogue-top{
    width: 100%;
    height: .5rem;
    img{
        width: .17rem;
        margin: .14rem .14rem;
    }
}
.catalogue-bottom{
    width: 100%;
    height: 5.3rem;
    margin: 0 auto;
    background: url("../assets/catalogue/小猫@2x.png") no-repeat center / cover;
    position: relative;
    .text{
        position: absolute;
        top: 3.2rem;
        left: 1.2rem;
        div{
            height: .41rem;
            width: 1.62rem;
            position: relative;
            line-height: .41rem;
            text-align: right;
            font-size: .12rem;
            &:nth-child(5){
                font-size: .15rem;
            }

            input{
                height: .36rem;
                width: 1.32rem;
                border: none;
                outline: none;
                font-size: .12rem;
                border-bottom:#322516 .01rem solid ;
                padding-left: .3rem;
                background: rgba( 0,0,0,0);
            }
            img{
                width: .16rem;
                position: absolute;
                left: 0;
                top: .1rem;
            }
            button{
                height: .36rem;
                width: 1.32rem;
                margin-right: .15rem;
                background-color: #b47c50;
                border-radius: .15rem;
                border: none;
                color: white;
            }
        }
    }
}
</style>