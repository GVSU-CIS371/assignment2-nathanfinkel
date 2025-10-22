<template>
  <div class="syrup">
    <div :style="{ backgroundColor: type.color,width: '100%', height: '100%'}"></div>
  </div>
</template>

<script setup lang="ts">
type Props = {
  type: {
    id: string;
    name: string;
    color: string;
  };
};
defineProps<Props>();
  </script>
<style lang="scss" scoped>
.syrup {
  transform: translateY(400%);
  background-color: #c6c6c6;
  position: relative;
  width: 100%;
  height: 20%;
  animation: pour-tea 2s 1s forwards;
  z-index: 2;
}
</style>
