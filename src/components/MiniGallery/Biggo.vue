<template>
  <div class="flex justify-center shadow-sm">
    <div>
      <img :src="item.image_url" alt />
      <div class="p-2 text-3xl">{{ item.title }}</div>
      <div class="p-2">{{ item.description }}</div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Biggo',
  props: {
    item: Object,
  },

  data: () => ({
    title: 'Judul 1',
    description: 'lorem ipsum',
    image_url: 'https://placehold.it/300?text=gambar1',
  }),
}
</script>
