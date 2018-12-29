<template>
  <section class="post-list">
    <PostPreview
      id="1"
      :is-admin="isAdmin"
      thumbnail="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSfKqgVZkNSm4SwUGuR94lDPfijbyY6SO2ezJeddc37sSilFOTu"
      title="hello there!"
      previewText="this is my first post!"
    />
    <PostPreview
      id="2"
      :is-admin="isAdmin"
      thumbnail="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSfKqgVZkNSm4SwUGuR94lDPfijbyY6SO2ezJeddc37sSilFOTu"
      title="hello there! 2"
      previewText="this is my second post!"
    />
    <PostPreview
      id="3"
      :is-admin="isAdmin"
      thumbnail="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSfKqgVZkNSm4SwUGuR94lDPfijbyY6SO2ezJeddc37sSilFOTu"
      title="hello there! 3"
      previewText="this is my third post!"
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

<style scoped>
.post-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>
