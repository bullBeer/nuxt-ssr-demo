<!--子路由文件名必须为index父级页面才能默认展示第一个子路由内容-->
<template>
  <div>
    <h3>{{title}}</h3>
  </div>
</template>

<script>
export default {
  data() {
    return {
      title: '首页'
    }
  }
}
</script>
