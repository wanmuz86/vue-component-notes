<template>
<div class="card p-5 bg-light m-3">
 <article>
 <h2>{{blog.title}}</h2>
 <h6>{{blog.subtitle}}</h6>
 <p>{{blog.content}}</p>
 </article>
 </div>
</template>

<script>

export default {
 name: 'Blog',
 props:['blog']
 }
</script>

<style>

</style>


