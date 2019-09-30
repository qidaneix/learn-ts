<template>
  <div class="piece">X</div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';

@Component({
  components: {},
})
export default class App extends Vue {}
</script>

<style lang="scss" scoped>
.piece {
  display: inline-block;
  width: 100%;
  height: 100%;
}
</style>
