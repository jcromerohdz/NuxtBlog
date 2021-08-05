<template>
  <div class="admin-post-page">
    <section class="update-form">
      <AdminPostForm
        :post="loadedPost"
      />
    </section>
  </div>
</template>

<script>
import AdminPostForm from '@/components/Admin/AdminPostForm'

export default {
  components: {
    AdminPostForm
  },
  data () {
    return {
      loadedPost: {
        author: 'Christian',
        title: 'My aweson post',
        content: 'Super amazing, thanks for that!',
        thumbnailLink: 'https://www.hydrocarbons-technology.com/wp-content/uploads/sites/9/2020/09/shutterstock_1152185600-1440x1008-1-857x600.jpg'
      }
    }
  }

}
</script>

<style>
.update-form {
  width: 90%;
  margin: 20px auto;
}

@media (min-width: 768px) {
  .update-form {
    width: 500px;
  }
}
</style>
