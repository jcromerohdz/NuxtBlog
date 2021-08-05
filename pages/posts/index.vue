<template>
  <div class="post-page">
    <section>
      <h1>Hello</h1>
    </section>
    <PostList />
  </div>
</template>

<script>
import PostList from '@/components/Posts/PostList.vue'

export default {
  components: {
    PostList
  }

}
</script>

<style scoped>
.posts-page {
  display: flex;
  justify-content: center;
  align-items: center;
}

</style>
