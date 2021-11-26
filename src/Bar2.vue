<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
import { defineProps } from 'vue';
const props = defineProps({
  gdp: Array,
});
</script>

<template>
  <div class="bar2">
    <div class="item">
      <label>美国 21.428</label>
      <div class="bar" style="background: #374451; width: 400px"></div>
    </div>
    <div class="item">
      <label>中国 14.343</label>
      <div class="bar" style="background: #b34335; width: 267.743px"></div>
    </div>
  </div>
</template>


<style>
.bar2 {
  width: 600px;
  box-sizing: border-box;
  margin: 3em;
  position: relative;
}
.bar2::before {
  content: '';
  display: block;
  width: 1px;
  height: 100%;
  position: absolute;
  background: #666;
  left: 50%;
}
.item {
  display: flex;
  height: 35px;
  line-height: 35px;
  margin: 1em 0;
  position: relative;
  justify-content: center;
  color: #fff;
}
.bar {
  width: 100px;
  height: 100%;
  margin-right: 1em;
  flex: 0 0 auto;
}
.item label {
  position: absolute;
  left: 50%;
  transform: translateX(-50%);
  text-shadow: 0 0 3px rgba(0, 0, 0, 0.5);
}
</style>
