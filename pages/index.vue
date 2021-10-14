<template>
  <div>
    <app-header />
    <div class="main">
      <nuxt-child/>
    </div>
    <app-footer />
  </div>
</template>

<script>
export default {
  
}
</script>

<style scoped>
  .main{
    padding: 20px;
    min-height: 800px;
    text-align: center;
  }
</style>


