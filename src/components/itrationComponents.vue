<script setup>
import {ref} from 'vue';
const books=ref({
  "books": [
    {
      "title": "To Kill a Mockingbird",
      "author": "Harper Lee",
      "genre": "Fiction",
      "year": 1960,
      "isbn": "9780061120084"
    },
    {
      "title": "1984",
      "author": "George Orwell",
      "genre": "Dystopian Fiction",
      "year": 1949,
      "isbn": "9780451524935"
    },
    {
      "title": "The Great Gatsby",
      "author": "F. Scott Fitzgerald",
      "genre": "Fiction",
      "year": 1925,
      "isbn": "9780743273565"
    },
    {
      "title": "Pride and Prejudice",
      "author": "Jane Austen",
      "genre": "Romance",
      "year": 1813,
      "isbn": "9780141439518"
    }
  ]
}
);

</script>

<template>

<ul v-for="(book,index) in books" :key="index">
    
   <ul v-for="({title,author,genre,year,isbn}) in book" >
   <li>Title:{{title}}</li>
   <li>Author:{{author}}</li>
   <li>Genre:{{genre}}</li>
   <li>Year:{{year}}</li>
   <li>ISBN:{{isbn}}</li>
   </ul>

</ul>


<ul v-for="(number,index) in 5" :key="index">
<li>Number:{{number}}</li>

</ul>

</template>