<template>
  <div class="admin-post-page">
    <section class="update-form">
      <AdminPostForm :post="loadedPost"/>
    </section>
  </div>
</template>

<script>
import AdminPostForm from "@/components/Admin/AdminPostForm";
export default {
  layout: 'admin',
  components: {
    AdminPostForm
  },
  data() {
    return {
      loadedPost: {
        author: "wtildestar",
        title: "Мое приложение",
        content: "Очень круто, спасибо! ",
        thumbnailLink:
          "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSfKqgVZkNSm4SwUGuR94lDPfijbyY6SO2ezJeddc37sSilFOTu"
      }
    };
  }
};
</script>

<style scoped>
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
