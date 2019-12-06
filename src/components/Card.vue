<template>
  <div class="card">
    <slot/>
  </div>
</template>

<script>
export default {
  name: 'Card',
};
</script>

<style scoped lang="scss">
.card {
  border-radius: 10px;
  //box-shadow: 0 5px 5px black;
  padding: 20px;
  box-shadow: rgba(0, 0, 0, 0.2) 0 3px 5px -1px,
    rgba(0, 0, 0, 0.14) 0 5px 8px 0,
    rgba(0, 0, 0, 0.12) 0 1px 10px 0;

  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
