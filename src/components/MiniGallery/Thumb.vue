<template>
  <div @click="$emit('setActive', item)" class="bg-white shadow-sm">
    <img :src="item.image_url" alt />
    <div class="text-center text-xs p-2">{{ item.title }}</div>
  </div>
</template>

<script>
export default {
  name: 'Thumb',
  props: {
    item: Object,
  },
}
</script>
