<template>
  <section class="posts-list">
    <PostPreview
      id="1"
      :is-admin="isAdmin"
      thumbnail="https://rhmagazine.pt/wp-content/uploads/2021/03/techh.png"
      title="Hello There!"
      preview-text="This is my first post"
    />
    <PostPreview
      id="2"
      :is-admin="isAdmin"
      thumbnail="https://rhmagazine.pt/wp-content/uploads/2021/03/techh.png"
      title="Hello There! 2"
      preview-text="This is my second post"
    />
    <PostPreview
      id="3"
      :is-admin="isAdmin"
      thumbnail="https://rhmagazine.pt/wp-content/uploads/2021/03/techh.png"
      title="Hello There! 3"
      preview-text="This is my third post"
    />
  </section>
</template>

<script>
import PostPreview from '@/components/Posts/PostPreview'

export default {
  components: {
    PostPreview
  },
  props: {
    isAdmin: {
      type: Boolean,
      default: false
    }
  }
}
</script>

<style>
.posts-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>
