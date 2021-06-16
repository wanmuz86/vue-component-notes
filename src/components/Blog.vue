<template>
<div class="card p-5 bg-light m-3">
 <article>
 <h2>{{blog.title}}</h2>
 <h6>{{blog.subtitle}}</h6>
 <p>{{blog.content}}</p>
 <button class="btn btn-danger" v-on:click="buttonPressed()">
     Delete</button>
 </article>
 </div>
</template>

<script>

export default {
 name: 'Blog',
 props:['blog'],
 methods:{
     buttonPressed(){
        this.$emit('deleted',this.blog.title)
     }
 }
 }
</script>

<style>

</style>


