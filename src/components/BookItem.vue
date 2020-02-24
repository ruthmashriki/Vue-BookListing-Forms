<template>
  <li> 
    <span v-if="book.finishedReading">Read</span>
    <span v-else="book.finishedReading">Not Read</span>
    {{book.title}} : {{book.author}}
   
  </li>
</template>

<script>
export default {
  name: 'BookItem',
  props: ['book'],
};
</script>

<style>
li {
  display: block;
  margin: 0 10px;
}
</style>