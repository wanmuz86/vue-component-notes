<template>
<div class="container">
  <main>
   <h2>Hello World</h2>
   
   <Blog v-for="blog in blogs" 
   :key="blog.title"
   v-bind="blog" />
   
  </main>
  </div>
</template>

<script>
import Blog from './Blog'
export default {
  name: 'Main',
  components: {
      Blog
  },
  data(){
      return {
          blogs:[
              {
                  "title":"My first blog",
                  "subtitle":"Happy to blog",
                  "content":"Wilkomen !!"
              },
              {
                  "title":"My second blog",
                  "subtitle":"Happy to blog again",
                  "content":"Best and still motivated !!"
              },
              {
                  "title":"My third blog",
                  "subtitle":"Happy to blog lagi",
                  "content":"Best and still motivated !!"
              }
          ]
      }
  }
  
}
</script>

<style>

</style>
