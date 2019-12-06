<template>
  <div class="home">
    <span class="logo">Paga<span class="green">.me</span></span>
    <HelloWorld/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue';

export default {
  name: 'home',
  components: {
    HelloWorld,
  },
};
</script>

<style scoped lang="scss">
.home {
  flex: 1;
  display: flex;
  flex-direction: column;
  //justify-content: center;
  align-items: center;
  width: 100%;
  min-height: 100vh;
}
.logo {
  padding: 32px;
  font-weight: bold;
  font-size: 52pt;
  color: #2c3e88;
  .green {
    color: #2c8850;
  }
}
</style>
