<template>
  <div>
    <p>新闻{{$route.params.id}}的页面</p>
   <div>为此页面设置了私有的title和description   便于SEO</div>
   <hr>
   <br>
   
   <p>我们使用了validate方法，并把params传递进去，然后用正则进行了校验，如果正则返回了true正常进入页面，如果返回false进入404页面。</p>
<br>
   <nuxt-link :to="{path:'/news'}">返回新闻列表</nuxt-link>
  </div>
</template>

<script>
export default {
  data() {
    return {
      title: "新闻详情!"
    };
  },
  head() {
    return {
      title: this.title,
      meta: [{ hid: "description", name: "description", content: "新闻详情啊" }]
    };
  },
  validate({ params }) {
    // Must be a number
    return /^\d+$/.test(params.id);
  }
};
</script>