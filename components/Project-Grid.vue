<template>
    <div class="project-grid">
      <nuxt-link to="projects/buddi" class="column-span-2 project-tile position-c">
        <div>
          <h3>Buddi</h3>
          <p class="text-muted text-small"><span class="is-highlighted text-small">2019 //</span> An express shopping and product information kiosk.</p>
        </div>
        <img src="@/assets/images/projects/ipad.png" alt="" class="fluid">
        <p class="text-muted text-small uppercase last">Project Details <i class="fal fa-long-arrow-right"></i></p>
      </nuxt-link>
      <nuxt-link to="projects/cully" class="project-tile position-a">
        <div>
          <h3>Cully Movie Bot</h3>
          <p class="text-muted text-small"><span class="is-highlighted text-small">2018 //</span> A Chatbot Channel to help Movie Theatres Sell Tickets.</p>
        </div>
        <img src="@/assets/images/projects/ipad.png" alt="" class="fluid">
        <p class="text-muted text-small uppercase last">Project Details <i class="fal fa-long-arrow-right"></i></p>
      </nuxt-link>
      <nuxt-link to="projects/motto" class="project-tile position-b">
        <div>
          <h3>Motto 20</h3>
          <p class="text-muted text-small"><span class="is-highlighted text-small">2018 //</span> A cryptocurrency dashboard experience.</p>
        </div>
        <img src="@/assets/images/projects/ipad.png" alt="" class="fluid">
        <p class="text-muted text-small uppercase last">Project Details <i class="fal fa-long-arrow-right"></i></p>
      </nuxt-link>
      <nuxt-link to="projects/rt-dashboard" class="project-tile position-d">
        <div>
          <h3>ResponseTek Dashboard</h3>
          <p class="text-muted text-small"><span class="is-highlighted text-small">2016 //</span> A voice of customer analytics dashboard.</p>
        </div>
        <img src="@/assets/images/projects/ipad.png" alt="" class="fluid">
        <p class="text-muted text-small uppercase last">Project Details <i class="fal fa-long-arrow-right"></i></p>
      </nuxt-link>
      <nuxt-link to="projects/rt-survey" class="project-tile position-e">
        <div>
          <h3>ResponseTek Surveys</h3>
          <p class="text-muted text-small"><span class="is-highlighted text-small">2016 //</span> A voice of customer program survey.</p>
        </div>
        <img src="@/assets/images/projects/ipad.png" alt="" class="fluid">
        <p class="text-muted text-small uppercase last">Project Details <i class="fal fa-long-arrow-right"></i></p>
      </nuxt-link>
    </div>
</template>
<script>
export default {
    
}
</script>
<style lang="scss" scoped>
.project-tile {
  background-color: #081014;
  background-image: url('../assets/images/logo-bg.png');
  background-image: url('../assets/images/logo-bg.png'), radial-gradient(50% 173%, rgba(255,255,255,0.00) 50%, #081014 100%);
  background-repeat: no-repeat;
  border: 1px solid rgba(255,255,255, 0.15);
  box-shadow: 0 0 14px 0 rgba(245, 166, 166, 0);
  // box-shadow: 0 0 14px 0 rgba(255,255,255,0.10);
  min-height: 300px;
  border-radius: 0.25rem;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  // transition: background-position 4000ms ease-in-out, background-size 5000ms ease-in-out , box-shadow 1500ms ease-in-out;
  transition: background-position 4000ms ease-in-out, background-size 5000ms ease-in-out , box-shadow 700ms ease-in-out, border 700ms ease-in-out;
  &:hover {
    box-shadow: 0 0 14px 0 rgba(255,255,255,0.20);
    border: 1px solid rgba(255,255,255, 0);
    img {
      animation: FloatingImage 2.5s ease-in-out infinite;   
    }
    a {
      transform: translateY(0px);
      opacity: 1;
    }
    h3, p {
      opacity: 1;
    }
  }
  h3 {
    padding: 1rem 1rem 0 1rem;
    opacity: 0.7;
  }
  p {
    margin: 0.5rem 0 0 1rem;
    opacity: 0.7;
    i {
      position: relative;
      top: 1px;
      margin-left: 3px;
    }
  }
  h3, p {
    transition: opacity 1.5s ease-in-out;
  }
  .last {
    transition: opacity 1.5s ease-in-out, transform 0.5s ease-in-out;
    opacity: 0;
    transform: translateY(5px);
    margin: 0 1rem 1rem auto;
  }
  img {
    margin: 1rem;
    align-self: center;
    transition: transform 300ms ease-in-out;
  }

  &.position-a {
    background-size: 1320%;
    background-position: 41% 38%;
    &:hover {
      background-size: 120%;
      background-position: 4% 38%;
    }
  }
  &.position-b {
    background-size: 1170%;
    background-position: 55% 6%;
    &:hover {
      background-size: 120%;
      background-position: 4% 38%;
    }    
  }
  &.position-c {
    background-size: 660%;
    background-position: 36% 66%; 
    &:hover {
      background-size: 650%;
      background-position: 30% 60%;
    }
  }
  &.position-d {
    background-size: 1850%;
    background-position: 35% 6%;
    &:hover {
      background-size: 120%;
      background-position: 4% 38%;
    }
  }
  &.position-e {
    background-size: 1090%;
    background-position: 76% 6%;
    &:hover {
      background-size: 120%;
      background-position: 4% 38%;
    }
  }
}

@keyframes FloatingImage {
  0% {
    transform: translateY(0px);
  }
  50% {
    transform: translateY(-5px);
  }
  100% {
    transform: translateY(0px);
  }
}



  .project-grid {
    display: grid;
    grid-template-columns: 1fr;
    grid-column-gap: 3rem;
    grid-row-gap: 3rem;
  }


  @media (min-width: 620px) {
  .project-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    .column-span-2 {
      grid-column: 1 / 3;
    }
  }
}






</style>
