<template>
  <div class="app-footer">
    <h3>{{title}}</h3>
  </div>
</template>

<script>
export default {
  data() {
    return {
      title: '底部'
    }
  }
}
</script>

<style scoped>
  .app-footer{
    height: 120px;
    background-color: #1da16e;
  }
  h3{
    color: #fff;
    font-size: 30px;
    text-align: center;
    line-height: 120px;
  }
</style>