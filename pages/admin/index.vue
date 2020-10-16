<template>
    <div class="AdminPage">
        <section class="NewPost">
            <button>Create Post</button>
        </section>
        <section class="ExistingPost">
            <h1>Existing Posts</h1>
            <PostList />
        </section>

    </div>
</template>

<style scoped>
.AdminPage {
  padding: 20px;
}

.NewPost {
  text-align: center;
  border-bottom: 2px solid #ccc;
  padding-bottom: 10px;
}

.ExistingPost h1 {
  text-align: center;
}
</style>