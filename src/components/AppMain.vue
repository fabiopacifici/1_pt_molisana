<script>
import ProductCard from "./ProductCard.vue";
import BlogPost from "./BlogPost.vue";
export default {
  name: 'AppMain.vue',
  components: {
    ProductCard,
    BlogPost
  },
  data() {
    return {
      posts: [
        {
          id: 1,
          content: 'Thisi sa content',
          subtitle: 'Sub title',
          img: 'https://picsum.photos/400/200',
          author: 'fab'
        },
        {
          id: 2,
          content: 'Thisi sa content',
          subtitle: 'Sub title',
          img: 'https://picsum.photos/400/200',
          author: 'fab'
        },
        {
          id: 3,
          content: 'Thisi sa content',
          subtitle: 'Sub title',
          img: 'https://picsum.photos/400/200',
          author: 'fab'
        }
      ],
      products: [
        {
          src: "https://www.lamolisana.it/wp-content/uploads/2021/04/1-spaghetto-quadrato.jpg",
          titolo: "N.4 Spaghetto Quadrato Bucato",
          tipo: "lunga",
          cottura: 6,
        },
        {
          src: "https://www.lamolisana.it/wp-content/uploads/2021/04/5-fettuccine.jpg",
          titolo: "N.5 Fettuccine",
          tipo: "lunga",
          cottura: 13,
        },
        {
          src: "https://www.lamolisana.it/wp-content/uploads/2021/04/6-linguine.jpg",
          titolo: "N.6 Linguine",
          tipo: "lunga",
          cottura: 12,
        },
        {
          src: "https://www.lamolisana.it/wp-content/uploads/2021/04/7-mezze-linguine.jpg",
          titolo: "N.7 Mezze Linguine",
          tipo: "lunga",
          cottura: 11,
        },
        {
          src: "https://www.lamolisana.it/wp-content/uploads/2021/04/11-spaghettino-quadrato.jpg",
          titolo: "n.11 Spaghettino Quadrato",
          tipo: "lunga",
          cottura: 9,
        },
        {
          src: "https://www.lamolisana.it/wp-content/uploads/2021/05/38-mezze-maniche.jpg",
          titolo: "N.38 Mezze maniche",
          tipo: "corta",
          cottura: 12,
        },
        {
          src: "https://www.lamolisana.it/wp-content/uploads/2021/05/44-sedani.jpg",
          titolo: "N.44 Sedani",
          tipo: "corta",
          cottura: 8,
        },
        {
          src: "https://www.lamolisana.it/wp-content/uploads/2021/05/49-sedani.jpg",
          titolo: "N.49 Sedanini",
          tipo: "corta",
          cottura: 8,
        },
        {
          src: "https://www.lamolisana.it/wp-content/uploads/2021/05/53-lumachine.jpg",
          titolo: "N.53 Lumachine",
          tipo: "corta",
          cottura: 12,
        },
        {
          src: "https://www.lamolisana.it/wp-content/uploads/2021/05/55-chifferi-rigati.jpg",
          titolo: "N.55 Chifferi rigati",
          tipo: "corta",
          cottura: 12,
        },
        {
          src: "https://www.lamolisana.it/wp-content/uploads/2021/05/58-misto-corto.jpg",
          titolo: "N.58 Misto corto",
          tipo: "corta",
          cottura: 9,
        },
        {
          src: "https://www.lamolisana.it/wp-content/uploads/2021/06/84-ditale-quadrato.jpg",
          titolo: "N.84 Ditale Quadrato",
          tipo: "cortissima",
          cottura: 12,
        },
      ]
    }
  }
}

</script>
<template>
  <main>



    <!--  <div class="container">
      <div class="row">
            <BlogPost :content="postContent" subtitle="This is a subtitle" img="https://picsum.photos/400/200" author="Fabio">
        </BlogPost>

        <BlogPost :content="post.content" :subtitle="post.subtitle" :img="post.img" :author="post.author"
          v-for="post in posts">
        </BlogPost>
      </div>
    </div> -->




    <section class="products">
      <div class="container">
        <h2>Products</h2>
        <div class="row">
          <div class="col-12 col-md-6 col-lg-4" v-for="product in products">
            <ProductCard :product="product" :src="product.src" :text="product.titolo"></ProductCard>
          </div>
        </div>
      </div>
    </section>

  </main>
</template>

<style scoped>
main
{
  min-height: 400px;
  background-image: url('/img/fondo-pag-speciali.jpg');
}
</style>