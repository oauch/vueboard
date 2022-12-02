<template>
  <PageHeader/> <!-- 헤더 컴포넌트 -->
  <router-view/> <!-- 페이지 이동 표시 --> 
  <PageFooter/>
</template>

<script>
import PageHeader from '@/components/PageHeader.vue'
import PageFooter from '@/components/PageFooter.vue'

export default {
  name: 'App',
  components: {
    PageHeader,
    PageFooter
  }
}
</script>

<style>
#app{
  font-family: Arial, Helvetica, sans-serif;
  -webkit-font-smoothing: anialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: salmon;
}

#nav{
  padding: 30px;
}

#nav a{
  font-weight: bold;
  color: salmon;
}

#nav a.router-link-exact-active{
  color: #42b983
}

</style>