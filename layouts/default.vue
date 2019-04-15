<template>
  <div class="background-img">
    <main-navigation/>
    <nuxt />
    <the-footer/>
  </div>
</template>

<script>
import MainNavigation from '~/components/Main-Navigation.vue';
import TheFooter from '~/components/Footer.vue';

export default {
    components: {
      MainNavigation,
      TheFooter,
      
  }
}
</script>


<style lang="scss">
@import 'normalize.css';
@import '@/assets/sass/_typography.scss';
@import '@/assets/sass/_buttons.scss';

body {
  margin: 0;
  background-color: #081014;
  color: #ffffff; 
  min-height: 100vh;
  
}
.container {
  padding: 100px 1rem 1rem 1rem;
  min-height: 100vh;
}

.background-img {
  background: url('../assets/images/logo-bg.png');
  background-repeat: no-repeat;
  background-size: 200%;
  background-position: 36% 12%;
}

  .grid {
    display: grid;
    grid-template-columns: 1fr;
    grid-column-gap: 3rem;
    grid-row-gap: 2rem;
  }

@media (min-width: 620px) {
  .grid {
    display: grid;
    grid-template-columns: 2fr 1fr;
  }
}


.fluid {
  max-width: 100%;
  height: auto;

}
</style>
