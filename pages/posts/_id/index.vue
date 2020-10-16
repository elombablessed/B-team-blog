<template>
    <div class="SinglePostsPage">
        <section class="Posts">
            <h1 class="PostsTitle">Title of Posts </h1>
            <div class="PostsDetails">
                <div class="PostsDetails">Last updated on Date</div>
                <div class="PostsDetails">Written by Name</div>
            </div>
            <p>Content of the Posts</p>
        </section>
        <section class="PostsFeedback">
            <p>Let me knoe what you think about the post, mail to <a href="mailto:blog@trials.com">blog@trials.com</a></p>
        </section>
    </div>
</template>
<style scoped>
.SinglePostsPage {
  padding: 30px;
  text-align: center;
  box-sizing: border-box;
}

.Posts {
  width: 100%;
}

@media (min-width: 768px) {
  .Posts {
    width: 600px;
    margin: auto;
  }
}

.PostsTitle {
  margin: 0;
}

.PostsDetails {
  padding: 10px;
  box-sizing: border-box;
  border-bottom: 3px solid #ccc;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

@media (min-width: 768px) {
  .PostsDetails {
    flex-direction: row;
  }
}

.PostsDetails {
  color: rgb(88, 88, 88);
  margin: 0 10px;
}

.PostsFeedback a {
  color: red;
  text-decoration: none;
}

.PostsFeedback a:hover,
.PostsFeedback a:active {
  color: salmon;
}
</style>