<template>
  <div class="title">
    <p class="text-lg">Code as Policies:</p>
    <p>Language Model Programs for Embodied Control</p>
  </div>
  <AuthorInfo />
  <AbstractComp />
  <CodeBox />
</template>

<script>
import AuthorInfo from './components/AuthorInfo.vue'
import AbstractComp from './components/AbstractComp.vue'
import CodeBox from './components/CodeBox.vue'

export default {
  name: 'App',
  components: {
    AuthorInfo, CodeBox, AbstractComp
  }
}
</script>

<style scoped>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
