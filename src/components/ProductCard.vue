<script>
export default {
  name: 'ProductCard',
  /* props: ['product'], */
  props: {
   /*  product: Object, */
    src: String,
    text: String,
  }
}
</script>

<template>
  <div class="product">
    <!--  <img :src='product.src' alt='' />
    <h3>{{ product.text }}</h3> -->
    <img :src='src' alt='' />
    <h3>{{ text }}</h3>
  </div>
</template>


<style scoped>
.product {
  height: 100%;
  background-color: var(--mol-light);
  border-radius: 1rem;
  transition: all 1s;
  &:hover {
    filter: drop-shadow(0 0 10px #002d75);
  }
  & img {
    border-top-left-radius: 1rem;
    border-top-right-radius: 1rem;
  }
  & h3 {
    padding: 1rem;
  }
  
  
}

</style>