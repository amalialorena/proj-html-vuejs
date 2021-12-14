<template>
  <div>
      <section class="new-arrivals">
          new arrivals
      </section>
       <section class="quotes">
          quotes
      </section>
      <section class="blog">
          blog
      </section >
      <section class="products">
          products
      </section>
      <section class="logos">
          logos
      </section>
  </div>
</template>

<script>
export default {
  name: 'Main',
  components: {
      
  }
}
</script>


<style scoped lang="scss">
    .featured {
        height: 100vh;   
    }
    .collections {
        height: 60vh;
        background-color: grey;
    }
    .best-seller {
        height: 60vh;
    }
    .offers {
        height: 50vh;
        background-color: grey;
    }
    .new-arrivals {
        height: 100vh;
    }
    .quotes {
        background-color: grey;
        height: 55vh;
    }
    .blog {
        height: 80vh;
    }
    .products {
        height: 60vh;
    }
    .logos {
        height: 30vh;
        background-color: grey;
    }

</style>