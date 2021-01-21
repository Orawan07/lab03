<template>
<div class="book-item">
  <h1>{{book.title}}</h1>

  <img v-bind:src="book.thumbnailUrl" /><br/>
  <b>Author:</b> {{book.author}} <br/>
  <b>Categoty:</b> {{book.category}} <br/>
  <b>ISBN:</b> {{book.isbn}} <br/>
  <b>Pages:</b> {{book.pageCount}} <br/>
  <b>Description:</b><br/>
  <p>{{book.shortDescription}}</p>  


</div>
    
</template>



<script>

export default {
  name: 'BookItem',
  components: {
    
  },
  props:["book"]

}
</script>




<style>
.book-item{
    overflow: auto;
    text-align: center;
    background-color: antiquewhite;
    padding: 10px;
    border: 1px bisque;
}


</style>