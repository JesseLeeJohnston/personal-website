<template>
<div class="container">

  <div class="hero-text">
    <p class="lead">Hi, I’m Jesse, a UX Designer with a passion for building web applications that customers love to use.<br/>I believe rapid prototyping and feedback cycles help achieve the best end product.</p>
  </div>


  <div class="grid">
    <project-grid/>
    <div>

      <div class="blog-post">
        <nuxt-link to="/">
          <h3>
            Types Of Cookware Pots And Pans
          </h3>        
        </nuxt-link>
        <div class="space-between-text uppercase">
          <p class="text-small text-muted">April 20, 2019</p>
        </div>        
      </div>

      <div class="blog-post">
        <nuxt-link to="/">
          <h3>
            Gas Grill Burners Getting To Know You
          </h3>
        </nuxt-link>
        <div class="space-between-text uppercase">
          <p class="text-small text-muted">April 19, 2019</p>
        </div>        
      </div>

      <div class="blog-post">
        <nuxt-link to="/">
          <h3>
            Fun Grill Sizzle
          </h3>
        </nuxt-link>
        <div class="space-between-text uppercase">
          <p class="text-small text-muted">April 18, 2019</p>
        </div>        
      </div>

      <div class="blog-post">
        <nuxt-link to="/">
          <h3>
            Barbecue Sauce For A Perfect Barbeque
          </h3>
        </nuxt-link>
        <div class="space-between-text uppercase">
          <p class="text-small text-muted">April 17, 2019</p>
        </div>        
      </div>

      <div class="blog-post">
        <nuxt-link to="/">
          <h3>
            Fun Grill Sizzle
          </h3>
        </nuxt-link>
        <div class="space-between-text uppercase">
          <p class="text-small text-muted">April 18, 2019</p>
        </div>        
      </div>

      <nuxt-link to="blog" class="button">
        View All
      </nuxt-link>


    </div>
  </div>

</div>


</template>

<script>
import ProjectGrid from '~/components/Project-Grid.vue';

export default {
  components: {
    ProjectGrid
  },
  data() {
    return {
      showNav: false,
    }
  }
}
</script>

<style lang="scss">

.hero-text {
  text-align: center;
  padding: 8rem 0rem;
  margin: 0 auto;
  max-width: 1200px;
}

.blog-post {
  margin-bottom: 2.6rem;
}
</style>
