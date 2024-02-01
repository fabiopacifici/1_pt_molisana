<script>
export default {
  name: 'BlogPost',
  props: ['content', 'subtitle', 'img', 'author']
}
</script>

<template>
  <div class="col-4">
    <div class="post">
      {{ content }}
      {{ subtitle }}
      <img :src="img" alt="">
      <div class="author">{{ author }}</div>
    </div>
  </div>
</template>

<style scoped></style>