<template>
  <div>
    <Biggo :item="activeItem" />

    <div class="flex">
      <div v-for="(item, index) in items" :key="index" class="w-1/4 m-2">
        <Thumb :item="item" @setActive="setActive" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    items: {
      type: Array,
      default: () => [],
    },
  },

  components: {
    Biggo: () => import('./Biggo'),
    Thumb: () => import('./Thumb'),
  },

  data: () => ({
    activeItem: {},
  }),

  methods: {
    setActive(item) {
      this.activeItem = item
    },
  },
}
</script>
