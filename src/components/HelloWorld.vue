<template>
  <Card class="container">
    <div class="header">
      <font-awesome-icon icon="arrow-left"/>
      <span class="handle">
        @jack
      </span>
      <font-awesome-icon :icon="['far', 'bookmark']" :style="{ opacity: '1' }"/>
    </div>
    <div class="qr">
      <QR></QR>
    </div>
    <div class="address">
      1F1tAaz5x1HUXrCNLbtMDqcw6o5GNn4xqX
      <font-awesome-icon icon="copy" :style="{ color: '#2c3e50' }"/>
    </div>
  </Card>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';
import QR from '@/components/QR.vue';
import Card from '@/components/Card.vue';
@Component({
  components: { QR, Card },
})
export default class HelloWorld extends Vue {
  @Prop() private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.container {
  display: flex;
  //justify-content: space-between;
  align-items: center;
  //flex: 1;
}
.header {
  width: 100%;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  flex: 1;
}
.handle {
  font-weight: bold;
}
.qr {
  //background-color: #dadff2;
  //padding: 10px 10px;
  //border-radius: 10px;
}
.address {
  background-color: #dadff2;
  padding: 5px 10px;
  border-radius: 10px;
}
</style>
