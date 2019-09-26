<template>
  <div class="home">
    <nav-component></nav-component>
    <div class="nav">
      <div class="show">
        <a v-for="(item, index) in texts" :href="item.href" :key="index">{{item.text}}</a>
      </div>
    </div>
    <agile class="agile" :dots="true" :autoplay="true" :infinite="true" :autoplay-speed="3000">
      <div v-for="(item,index) in banner" :key="index"  class="slide">
        <h3  :style="{backgroundImage: 'url(' +item.url + ')'} "></h3>
      </div>
    </agile>
    <div class="image">
      <img v-for="(item,index) in images"  :src="item.site">
      <span v-for="(item,index) in images" >{{item.text}}</span>
    </div>
    <div class="content">
      <div id="one" class="content1">
        <div class="title">精选商品</div>
        <agile class="agile2" :dots="true" :infinite="false">
          <div class="slide">
            <h3>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
            </h3>
          </div>
          <div class="slide">
            <h3>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
            </h3>
          </div>
          <div class="slide">
            <h3>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
            </h3>
          </div>
          <div class="slide">
            <h3>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
            </h3>
          </div>
        </agile>
      </div>
      <div id="two" class="content1">
        <div class="title">罐头零食</div>
        <agile class="agile2" :dots="true" :infinite="false">
          <div class="slide">
            <h3>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
            </h3>
          </div>
          <div class="slide">
            <h3>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
            </h3>
          </div>
          <div class="slide">
            <h3>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
            </h3>
          </div>
          <div class="slide">
            <h3>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
            </h3>
          </div>
        </agile>
      </div>
      <div id="three" class="content1">
        <div class="title">精选商品</div>
        <agile class="agile2" :dots="true" :infinite="false">
          <div class="slide">
            <h3>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
            </h3>
          </div>
          <div class="slide">
            <h3>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
            </h3>
          </div>
          <div class="slide">
            <h3>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
            </h3>
          </div>
          <div class="slide">
            <h3>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
            </h3>
          </div>
        </agile>
      </div>
      <div id="four" class="content1">
        <div class="title">精选商品</div>
        <agile class="agile2" :dots="true" :infinite="false">
          <div class="slide">
            <h3>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
            </h3>
          </div>
          <div class="slide">
            <h3>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
            </h3>
          </div>
          <div class="slide">
            <h3>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
            </h3>
          </div>
          <div class="slide">
            <h3>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
            </h3>
          </div>
        </agile>
      </div>
      <div id="five" class="content1">
        <div class="title">精选商品</div>
        <agile class="agile2" :dots="true" :infinite="false">
          <div class="slide">
            <h3>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
            </h3>
          </div>
          <div class="slide">
            <h3>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
            </h3>
          </div>
          <div class="slide">
            <h3>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
            </h3>
          </div>
          <div class="slide">
            <h3>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
              <div class="text">
                <img src="../assets/home/519281783059485516@2x.png">
                <p>加拿大原装进口 原始猎食渴望...</p>
                <p><span>￥</span><span>760</span><span>已售出13227</span></p>
              </div>
            </h3>
          </div>
        </agile>
      </div>
    </div>
  </div>

</template>

<script>
import NavComponent from "../components/header-Component";
import img1 from '../assets/home/u=194457569,2178415267&fm=26&gp=0@2x.png'
import img2 from '../assets/home/u=18720470,1837941433&fm=15&gp=0@2x.png'
import img3 from '../assets/home/u=937199075,1690847182&fm=15&gp=0@2x.png'
import img4 from '../assets/home/u=809093551,555726347&fm=26&gp=0@2x.png'
import imgs from '../assets/home/banner@2x.png'

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
          images:[
              {
              site: img1,text:'新人专区'
          },{
              site:img2,text:'今日特卖'
          },{
              site:img3,text:'今日热销'
          },{
              site:img4,text:'今日上新'
          }],
          banner:[
              {
            url:imgs
          },{
              url:imgs
          },{
              url:imgs
          },{
              url:imgs
          },{
              url:imgs
          },{
              url:imgs
          },],
      }
    }
}
</script>
<style lang="scss">
  body{
    background-color: #f7f5ef;
  }
  .nav::-webkit-scrollbar {
    display: none;
  }
.home .nav{
  height: .44rem;
  background:rgba(255,255,255,1);
  overflow-x: auto;
  position: sticky;
  z-index: 4;
  top: 0;
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

.agile{
  h3{
    height: 1.35rem;
    width: 100%;
    background: no-repeat center / cover;
  }
  .agile__actions{

 .agile__nav-button{
   display: none;
 }
  .agile__dots{
    margin: 0 auto;
    margin-top: -.26rem;
    z-index: 2;
    li{
      font-size: .1rem;
      &.agile__dot--current{
        button{
          background-color: #6a3906;
        }
      }
      button{
        height: .08rem;
        width: .08rem;
        margin-right: .08rem;
        border:  0 solid;
        border-radius: .1rem;
        background-color: #fff;
      }
    }
  }
  }
}
.image{
  background-color: #f7f5ef;
  width: 100%;
  height: 1.3rem;
  img{
    display: block;
    float: left;
    margin: .21rem .16rem .01rem .16rem;
    height: .6rem;
  }
  span{
    display: block;
    float: left;
    margin: 0 .20rem .16rem .20rem;
    height:0.13rem;
    font-size:0.13rem;
  }
}

.content1{
  height: 5.18rem;
  width: 100%;
  margin-bottom: .2rem;
  background-color: #fff;
  .title{
    font-size: .14rem;
    font-weight: 400;
    color:rgba(51,51,51,1);
    margin-left: .14rem;
    /*margin-top: .2rem;*/
    padding-top: .1rem;
  }
  .agile.agile2{
    .agile__dots{
      margin: 0 auto;
      margin-top: .1rem;
      z-index: 2;
      .agile__dot{
         button{
           border: #ab7246 1px solid ;
        }
      }
    }
    h3{
      width: 100%;
      /*height: 4.5rem;*/
      .text{
        margin: 0 .1rem;
        width: 1.58rem;
        height: 2.3rem;
        float: left;
        img{
          width: 1.48em;
        }
        p{
          color: #333;
          line-height: .2rem;
          width: 1.48rem;
          font-weight: 400;
          margin-left: .1rem;
          font-size: .15rem;
          margin-bottom: .1rem;
          span:nth-child(1){
            float: left;
          }
          span:nth-child(2){
            float: left;
          }
          span:nth-child(3){
            float: right;
          }
        }
      }
    }
  }
}
</style>