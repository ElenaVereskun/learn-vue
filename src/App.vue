<template>
  <div class="app">
    <post-form @create="createPost" />
    <post-list :posts="posts" />
  </div>
</template>
<script>
import PostForm from "@/components/PostForm.vue";
import PostList from "@/components/PostList.vue";
export default {
  components: {
    PostForm,
    PostList,
  },
  data() {
    return {
      posts: [
        { id: 1, title: "JS", body: "Описание поста" },
        { id: 2, title: "JS 2", body: "Описание поста 2" },
        { id: 3, title: "JS 3", body: "Описание поста 3" },
        { id: 4, title: "JS 3", body: "Описание поста 4" },
      ],
    };
  },
  methods: {
    createPost(post) {
      this.post.push(post);
    },
  },
};
</script>
<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.app {
  padding: 20px;
}
</style>
