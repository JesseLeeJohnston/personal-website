<template>
  <div class="container" style="padding-top: 10rem;">
    <h2>Hi, I'm Jesse!</h2>
    <div class="grid">
      <div>
        <p
          class="lead"
        >I didn’t develop the first vaccine, or create Ave Maria, however I always strive for more knowledge and experience. Now, I am a product designer residing in beautiful Vancouver, Canada. With a background in creative advertising and web development, I’ve boosted and merged the skills by having the opportunity to design a software that is used by Rogers, T-Mobile, and Vodaphone.</p>

        <p
          class="lead"
        >In my spare time away from the office I like to try new restaurants and brews. I love hanging out with my wife and bike riding along the beautiful Vancouver seawall.</p>
      </div>

      <div>
        <img src="@/assets/images/Jesse-Headshot.jpg" class="fluid">
      </div>
    </div>

    <div style="margin-top: 4rem;">
      <h2>My Experience</h2>

      <ul class="timeline">
        <!-- Item 1 -->
        <li>
          <div class="direction-r">
            <div class="flag-wrapper">
              <h3 class="flag">Buddi</h3>
            </div>
            <div class="time-wrapper">2018 - Present</div>
            <div class="desc text-muted text-small">Co-founder VP of Product & Design</div>
          </div>
        </li>

        <!-- Item 2 -->
        <li>
          <div class="direction-l">
            <div class="flag-wrapper">
              <h3 class="flag">Cully</h3>
            </div>
            <div class="time-wrapper">2017 - 2018</div>
            <div class="desc text-muted text-small">Product Design Lead</div>
          </div>
        </li>

        <!-- Item 3 -->
        <li>
          <div class="direction-r">
            <div class="flag-wrapper">
              <h3 class="flag">ResponseTek</h3>
            </div>
            <div class="time-wrapper">2014 - 2017</div>
            <div class="desc text-muted text-small">User Experience Designer</div>
          </div>
        </li>

        <!-- Item 3 -->
        <li>
          <div class="direction-l">
            <div class="flag-wrapper">
              <h3 class="flag">Brandspank</h3>
            </div>
            <div class="time-wrapper">2009 - 2014</div>
            <div class="desc text-muted text-small">Digital Strategy</div>
          </div>
        </li>

        <!-- Item 3 -->
        <li>
          <div class="direction-r">
            <div class="flag-wrapper">
              <h3 class="flag">Seneca College</h3>
            </div>
            <div class="time-wrapper">2007 - 2009</div>
            <div class="desc text-muted text-small">Creative Advertising Diploma</div>
          </div>
        </li>
      </ul>

      <router-link to="/" class="button">
        View My Resume
      </router-link>

    </div>
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss" scoped>
.timeline {
  position: relative;
  width: 660px;
  margin: 0 auto;
  margin-top: 20px;
  padding: 1em 0;
  list-style-type: none;
}
.timeline:before {
  position: absolute;
  left: 50%;
  top: 0;
  content: " ";
  display: block;
  width: 2px;
  height: 100%;
  margin-left: -1px;
  background: #1e3744;
  background: linear-gradient(
    to bottom,
    rgba(80, 80, 80, 0) 0%,
    #1e3744 8%,
    #101f27 92%,
    rgba(80, 80, 80, 0) 100%
  );
  z-index: 5;
}
.timeline li {
  padding: 2rem 0;
}
.timeline li:after {
  content: "";
  display: block;
  height: 0;
  clear: both;
  visibility: hidden;
}
.direction-l {
  position: relative;
  width: 300px;
  float: left;
  text-align: right;
}
.direction-r {
  position: relative;
  width: 300px;
  float: right;
}
.flag-wrapper {
  position: relative;
  display: inline-block;
  text-align: center;
}
.direction-l .flag:before,
.direction-r .flag:before {
  position: absolute;
  top: 50%;
  right: -40px;
  content: " ";
  display: block;
  width: 12px;
  height: 12px;
  margin-top: -10px;
  background: #fff;
  border-radius: 10px;
  border: 4px solid #208fc6;
  z-index: 10;
}

.direction-r .flag:before {
  left: -40px;
}

.direction-l .flag:after {
  content: "";
  position: absolute;
  left: 100%;
  top: 50%;
  height: 0;
  width: 0;
  margin-top: -8px;
  border: solid transparent;
  border-width: 8px;
  pointer-events: none;
}

.direction-r .flag:after {
  content: "";
  position: absolute;
  right: 100%;
  top: 50%;
  height: 0;
  width: 0;
  margin-top: -8px;
  border: solid transparent;
  border-width: 8px;
  pointer-events: none;
}
.time-wrapper {
  margin: 0.5rem 0rem;
  line-height: 1rem;
  color: #208fc6;
}
.desc {
  margin: 1rem 0;
}

.direction-r .desc {
  margin: 1rem 0;
}

/* ================ Timeline Media Queries ================ */

@media screen and (max-width: 660px) {
  .timeline:before {
    background: rgba(0, 0, 0, 0);
  }
  .timeline {
    width: 100%;
    padding: 4em 0 1em 0;
  }

  .timeline li {
    padding: 3em 0;
  }

  .direction-l,
  .direction-r {
    float: none;
    width: 100%;
    text-align: center;
  }

  .flag-wrapper {
    text-align: center;
  }

  .direction-l .flag:before,
  .direction-r .flag:before {
    position: absolute;
    top: -30px;
    left: 50%;
    content: " ";
    display: block;
    width: 12px;
    height: 12px;
    margin-left: -9px;
    border-radius: 10px;
  }

  .direction-l .flag:after,
  .direction-r .flag:after {
    content: "";
    position: absolute;
    left: 50%;
    top: -8px;
    height: 0;
    width: 0;
    margin-left: -8px;
    border-width: 8px;
    pointer-events: none;
  }

  .time-wrapper {
    display: block;
    position: relative;
  }

  .direction-l .time-wrapper {
    float: none;
  }

  .direction-r .time-wrapper {
    float: none;
  }

  .desc {
    position: relative;
    margin: 1em 0 0 0;
    padding: 1em;
    // background: rgb(245,245,245);
    -webkit-box-shadow: 0 0 1px rgba(0, 0, 0, 0.2);
    -moz-box-shadow: 0 0 1px rgba(0, 0, 0, 0.2);
    box-shadow: 0 0 1px rgba(0, 0, 0, 0.2);

    z-index: 15;
  }

  .direction-l .desc,
  .direction-r .desc {
    position: relative;
    margin: 1em 1em 0 1em;
    padding: 1em;

    z-index: 15;
  }
}
</style>
