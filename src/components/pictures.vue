<script setup>
import { Carousel } from 'flowbite-vue'
const pictures = [
  {
    'src': 'https://static.trip101.com/main_pics/200831/medium_webp.webp ',
    'alt': 'Picture 1',
  },
  {
    'src': 'https://upload.wikimedia.org/wikipedia/commons/thumb/2/23/Times_Square%2C_Seoul.jpg/800px-Times_Square%2C_Seoul.jpg',
    'alt': 'Picture 2',
  },
  {
    'src': 'https://media.timeout.com/images/103614349/750/422/image.jpg',
    'alt': 'Picture 3',
  },
  {
    'src': 'https://images.adsttc.com/media/images/5014/7a8e/28ba/0d39/5000/002a/newsletter/stringio.jpg?1414070050',
    'alt': 'Picture 4',
  },
  {
    'src': 'https://c8.alamy.com/comp/M78YFN/seoul-south-korea-august-17-2015-people-enjoing-their-free-time-at-M78YFN.jpg',
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


