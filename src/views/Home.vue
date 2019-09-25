<template>
  <div class="home">
    <nav-component></nav-component>
    <div class="nav">
      <div class="show">
        <a v-for="item in texts" :href="item.href">{{item.text}}</a>
      </div>

    </div>
  </div>
</template>

<script>
    import NavComponent from "../components/header-Component";
export default {
  name: 'home',
  components: {
      NavComponent

  },
    data() {
      return {
          texts:[
              {
                  href:'#one', text:'精选'
              },{
                  href:'#two', text:'猫粮'
              },{
                  href:'#three', text:'猫砂'
              },{
                  href:'#four', text:'罐头零食'
              },{
                  href:'#five', text:'猫爬架'
              }],
      }
    }
}
</script>
<style lang="scss">
  .nav::-webkit-scrollbar {
    display: none;
  }
.home .nav{
  height: .44rem;
  background:rgba(255,255,255,1);
  overflow-x: auto;
  .show{
    width: 120%;
    a{
      font-size:0.16rem;
      display: block;
      color:rgba(51,51,51,1);
      line-height:0.44rem;
      float: left;
      text-decoration: none;
      margin: 0 .21rem;
      font-weight:400;
    }
  }
}


</style>