<script setup>
import { Carousel } from 'flowbite-vue'
const pictures = [
  {
    'src': 'https://flowbite.s3.amazonaws.com/docs/gallery/featured/image.jpg',
    'alt': 'Picture 1',
  },
  {
    'src': 'https://flowbite.s3.amazonaws.com/docs/gallery/square/image-1.jpg',
    'alt': 'Picture 2',
  },
  {
    'src': 'https://flowbite.s3.amazonaws.com/docs/gallery/square/image-2.jpg',
    'alt': 'Picture 3',
  },
  {
    'src': 'https://flowbite.s3.amazonaws.com/docs/gallery/square/image-3.jpg',
    'alt': 'Picture 4',
  },
  {
    'src': 'https://flowbite.s3.amazonaws.com/docs/gallery/square/image-5.jpg',
    'alt': 'Picture 5',
  },
]

const props = defineProps({
    pictures: {
        type: Array,
        default() {
            return [
                {
                    'src': 'https://flowbite.com/docs/images/carousel/carousel-1.svg',
                    'alt': 'Picture 1',
                },
                {
                    'src': 'https://flowbite.com/docs/images/carousel/carousel-2.svg',
                    'alt': 'Picture 2',
                },
                {
                    'src': 'https://flowbite.com/docs/images/carousel/carousel-3.svg',
                    'alt': 'Picture 3',
                },
            ]
        },
    },
})

</script>
<template>
  <Carousel :pictures="pictures"></Carousel>
</template>


