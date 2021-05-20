<template>
  <li>{{ book.title }}:{{ book.author }}</li>
  <li v-for="book in books" :key="book.title">{{ book.title }}:{{ book.author }}</li>
</template>

<script>
export default {
  name: "BookItem",
  data() {
    return {
      props: ["book"],
    };
  },
};
</script>

<style>
li {
  display: block;
  margin: 0 10px;
}
</style>