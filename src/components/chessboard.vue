<template>
  <div class="container">
    <div class="item item-1">
      <piece></piece>
    </div>
    <div class="item item-2">2</div>
    <div class="item item-3">3</div>
    <div class="item item-4">4</div>
    <div class="item item-5">5</div>
    <div class="item item-6">6</div>
    <div class="item item-7">7</div>
    <div class="item item-8">8</div>
    <div class="item item-9">9</div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import piece from './piece.vue';

@Component({
  components: {
    piece,
  },
})
export default class App extends Vue {}
</script>

<style lang="scss" scoped>
.container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: repeat(3, 1fr);
  width: 96vw;
  height: 96vw;
  border: 1px solid #000;
  .item {
    font-size: 10vw;
    text-align: center;
    border: 1px solid #000;
  }
}
</style>
