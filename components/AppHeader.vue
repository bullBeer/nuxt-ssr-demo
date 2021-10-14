<template>
  <div class="app-header">
    <div class="header-bd">
      <div class="logo">Logo</div>
      <nav class="nav">
        <ul class="nav-list">
          <li v-for="(item, i) in navList" :key="i" :class="{current: $route.name === item.routerName}">
            <nuxt-link :to="{name: item.routerName}">{{item.label}}</nuxt-link>
          </li>
        </ul>
      </nav>
    </div>    
  </div>
</template>

<script>
export default {
  data() {
    return {
      navList: [
        {
          label: '首页',
          routerName: 'index', // 子路由初始展示路由名称必须为index(必须与路由文件名一致)
        },
        {
          label: '资讯中心',
          routerName: 'index-news',
        },
        {
          label: '产品业务',
          routerName: 'index-product',
        },
        {
          label: '公司资质',
          routerName: 'index-info',
        },
        {
          label: '关于我们',
          routerName: 'index-about',
        },
      ]
    }
  }
}
</script>

<style lang="less" scoped>
  .app-header{
    text-align: center;
    background-color: #25c88a;
    height: 60px;
  }
  .header-bd{
    margin: 0 auto;
    width: 1200px;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .logo{
    width: 120px;
    height: 40px;
    background-color: #1da16e;
    line-height: 40px;
    text-align: center;
    font-size: 24px;
    color: #fff;
    font-weight: bold;
  }
  .nav{
    flex: 1;
    
  }
  .nav-list{
    display: flex;
    justify-content: flex-end;
    li{
      font-size: 18px;
      &.current{
        background-color: #1da16e;
      }
    }
    a{
      width: 6em;
      height: 60px;
      display: flex;
      justify-content: center;
      align-items: center;
      color: #fff;
      text-decoration: none;
      outline: none;
    }
  }
</style>
