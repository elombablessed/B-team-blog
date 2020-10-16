<template>
    
      <nuxt-link :to="'/posts/' + id" class="PostsPreview">
        <article >
            <div 
            class="PostsThumbnail" 
            :style="{backgroundImage: 'url('+thumbnail+')'}"></div>
            <div class="PostsContent">
              <h1>{{title}}</h1>
              <p>{{preview}}</p>
            </div>
        </article>
      </nuxt-link>
</template>

<script>
export default {
    name: "PreviewPosts",
    props:{
        id:{
            type: String,
            required: true
        },
        thumbnail:{
            type: String,
            required: true
        },
        title:{
            type: String,
            required: true
        },
        preview:{
            type: String,
            required: true
        }
    }
}
</script>

<style scoped>



.PostsPreview {
  border: 1px solid #ccc;
  box-shadow: 0 2px 2px #ccc;
  background-color: white;
  width: 90%;
}

a {
  text-decoration: none;
  color: black;
}

@media (min-width: 850px) {
  .PostsPreview {
    width: 400px;
    margin: 10px;
  }
}

.PostsThumbnail {
  width: 100%;
  height: 200px;
  background-position: center;
  background-size: cover;
}

.PostsContent {
  padding: 10px;
  text-align: center;
}

a:hover .PostsContent,
a:active .PostsContent {
  background-color: #ccc;
}
</style>