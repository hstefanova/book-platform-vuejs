<template>
  <router-link :to="{ name: 'book', params: { bookId: book.id } }">
    <div class="book">
      <div
        class="book__image"
        :style="{ backgroundImage: `url(${book.image})` }"
      ></div>

      <h2>{{ book.title }}</h2>
    </div>
  </router-link>
</template>

<script>
export default {
  props: {
    book: Object
  }
}
</script>

<style scoped>
.book {
  text-align: center;
  border: 1px solid grey;
  padding: 20px 20px 10px;
  display: inline-block;
}
.book .book__image {
  width: 200px;
  height: 270px;
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center center;
}
</style>
