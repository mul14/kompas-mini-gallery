<template>
  <div id="app">

    <MiniGallery :items="galleries"/>

  </div>
</template>

<script>
export default {
  components: {
    MiniGallery: () => import('./components/MiniGallery/Index'),
  },

  data: () => ({
    galleries: [
      {
        title: 'Judul 1',
        description: 'lorem ipsum',
        image_url: 'https://placehold.it/300?text=gambar1',
      },{
        title: 'Judul 2',
        description: 'lorem ipsum',
        image_url: 'https://placehold.it/300?text=gambar2',
      },{
        title: 'Judul 3',
        description: 'lorem ipsum',
        image_url: 'https://placehold.it/300?text=gambar3',
      },{
        title: 'Judul 4',
        description: 'lorem ipsum',
        image_url: 'https://placehold.it/300?text=gambar4',
      }
    ]
  })

}
</script>
