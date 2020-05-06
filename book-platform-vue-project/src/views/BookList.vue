<template>
  <div>
    <h1>Books list</h1>

    <BaseBook v-for="book in books" :book="book" :key="book.id" />
  </div>
</template>

<script>
import BaseBook from '@/components/BaseBook.vue'

export default {
  data() {
    return {
      books: [
        {
          id: 1,
          title: 'Harry Potter',
          year: 'Aug 28 2018',
          author: 'J.K.Rowling',
          description: "It's a story about a young boy...",
          genre: 'fantasy',
          image:
            'https://images-eu.ssl-images-amazon.com/images/I/51OZerWcGCL.jpg'
        },

        {
          id: 2,
          title: 'Knife',
          year: 'Aug 28 2018',
          author: 'Nesbu',
          description: 'Knife is a story about...',
          genre: 'criminal',
          image:
            'https://images-na.ssl-images-amazon.com/images/I/31RCAoIEUbL._SX332_BO1,204,203,200_.jpg'
        },

        {
          id: 3,
          title: 'Rich, poor',
          year: 'Aug 28 2020',
          author: 'K.L.Shou',
          description: "It's a story about a family...",
          genre: 'novel',
          image: 'https://m.media-amazon.com/images/I/51-WiB-BePL.jpg'
        }
      ]
    }
  },
  components: {
    BaseBook
  }
}
</script>
