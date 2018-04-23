<template>
  <div>
    <h2>
      News Index Page
    </h2>
    <br>
    <p>     :to="{path:'/news/2'}"    :to="{name:'news-id',params:{id:5}}" 两种方式 </p>
    <br>
    <ul>
      <li><nuxt-link to="/">回到首页</nuxt-link></li>
      <li><nuxt-link :to="{path:'/news/a'}">新闻a  参数a不是数字，会跳到404</nuxt-link></li>
      <li><nuxt-link :to="{path:'/news/2'}">新闻2</nuxt-link></li>
      <li><nuxt-link :to="{path:'/news/3'}">新闻3</nuxt-link></li>
      <li><nuxt-link :to="{path:'/news/4'}">新闻4</nuxt-link></li>
      <li><nuxt-link :to="{name:'news-id',params:{id:5}}">新闻5</nuxt-link></li>      
    </ul>
  </div>
</template>