<template>
  <div>
    <ul>
      <!-- <li><a href="/">Home</a></li>
      <li><a href="/about">About</a></li>
      <li><a href="/news">News</a></li> -->
      <li><nuxt-link :to="{name:'index'}">Home</nuxt-link></li>
      <li><nuxt-link :to="{name:'about'}">About</nuxt-link></li>
      <li><nuxt-link :to="{path:'/user'}">User</nuxt-link></li>
      <li><nuxt-link :to="{name:'news',params:{newsId:1}}">News</nuxt-link></li>
    </ul>
  </div>
</template>

<script>
export default {};
</script>

<style></style>