<template>
  <div class="admin-post-page">
    <section class="update-form">
      <AdminPostForm :post="loadedPost" />
    </section>
  </div>
</template>

<script>
import AdminPostForm from "@/components/Admin/AdminPostForm";
export default {
  components: {
    AdminPostForm
  },

  data() {
    return {
      loadedPost: {
        author: "Shakil",
        title: "the title",
        content: "Supper amazing post",
        thumbnailLink:
          "https://static.pexels.com/photos/270348/pexels-photo-270348.jpeg"
      }
    };
  }
};
</script>

<style lang="stylus" scoped></style>