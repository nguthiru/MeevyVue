<template>
  <skeleton-vue>
    <section id="hero">
      <div class="col">
        <h1>
          Listen, Match and connect<br />
          instantly
        </h1>
        <p>
          Do you love music? Get to know your musical soulmates based of your
          taste. <br />
          Interact with them, share music and <a>more</a>. <br />
          <b>ALL FOR FREE!</b>
        </p>
        <div class="row">
          <a href="#"><img src="../assets/google-play-badge.png" alt="Google Play" class="download-badge" /></a>
          <a href="#"><img src="../assets/Available_on_the_App_Store_(black).png" alt="Google Play"
              class="download-badge" /></a>
        </div>
      </div>
      <img src="../assets/hero-image.svg" id="hero-image" alt="" class="section-image"/>
    </section>
    <section class="feature-section" id="features1">
      <div class="feature-icon">
        <img src="../assets/match-icon.png" alt="match" />
        <div class="col">
          <p>Matchmake through our algorithm</p>
          <p class="feature-tagline">DISCOVER</p>
        </div>
      </div>
      <article>
        <div class="feature-text col">
          <h2>Know Your Musical Soulmates</h2>
          <p class="feature-description">
            Discover your musical matches, view what brought you together.
            Artists, Tracks. <br />Send them and accept their requests to
            begin chatting.
          </p>
        </div>
        <div class="feature-image-content">
          <div class="feature-background"></div>
          <img src="../assets/movkup1.png" alt="" class="section-image mockup-image"/>
        </div>
      </article>
    </section>
    <section class="feature-section">
      <div class="feature-icon">
        <img src="../assets/message_icon.png" alt="match" />
        <div class="col">
          <p>Chat and send songs to friends</p>
          <p class="feature-tagline">CONNECT</p>
        </div>
      </div>
      <article>
        <div class="feature-text col">
          <h2>Connect with your friends</h2>
          <p class="feature-description">
            Casually chat with your friends and send spotify songs to each
            other. <br />
            begin chatting.
          </p>
        </div>
        <div class="feature-image-content">
          <div class="feature-background"></div>
          <img src="../assets/moclup2.png" alt="" class="section-image mockup-image"/>
        </div>
      </article>
    </section>
    <section class="feature-section">
      <div class="feature-icon">
        <img src="../assets/listen_icon.png" alt="match" />
        <div class="col">
          <p>Listen With Friends</p>
          <p class="feature-tagline">SYNC</p>
        </div>
      </div>
      <article>
        <div class="feature-text col">
          <h2>If you love it, show them</h2>
          <p class="feature-description">
            Use spots to share your currently playing to your daily story. Sync to friend's spots and listen to what
            they love.<br>They can also sync to yours.
            CREATE A SPOT.
          </p>
        </div>
        <div class="feature-image-content">
          <div class="feature-background"></div>
          <img src="../assets/mockup3.png" alt="" class="section-image mockup-image"/>
        </div>
      </article>
    </section>
  </skeleton-vue>
</template>

<script>
import SkeletonVue from '../components/Skeleton.vue';
export default {
  name: 'Home',
  components: {
    SkeletonVue
  }
}
</script>

<style>
section {
  scroll-snap-align: start;
  margin-top: 1em;
  height: 95vh;
}

#hero {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

#hero-image {
  height: 70vh;
}

#hero h1+p {
  margin: 1em 0;
  line-height: 2;
}

#hero h1 {
  text-transform: uppercase;
}

.align-center {
  align-items: center;
}

.download-badge {
  width: 10em;
}

#hero .download-badge {
  margin-right: 2em;
}

.sub-text {
  color: rgb(71, 71, 71);
  line-height: 2;
}

.mouse-scroll-item {
  position: fixed;
  bottom: 1em;
  left: 1em;
  pointer-events: none;
}

.mouse-body {
  display: block;
  position: relative;
  width: 25px;
  height: 60px;
  border: 3px solid grey;
  border-radius: 5em;
}

.mouse-wheel {
  background-color: grey;
  display: block;
  width: 7px;
  height: 7px;
  margin-left: auto;
  margin-right: auto;
  border-radius: 50%;
  margin-top: 0.3em;
  transition: all 1s;
}

@keyframes animate-wheel {
  0% {
    transform: translateY(10%);
    opacity: 1;
  }

  100% {
    transform: translateY(30%);
    opacity: 0;
  }
}

@keyframes enlarge {
  0% {
    transform: scale(0%);
  }

  100% {
    transform: scale(10%);
  }
}

.feature-image-content {
  position: relative;
  width: fit-content;
  margin-left: 4em;
}

.feature-background {
  width: 20vw;
  position: absolute;
  right: 0;
  bottom: 0;
  left: 0;
  z-index: -1;
  height: 50vh;
  background: rgba(255, 255, 255, 0.4);
  -webkit-backdrop-filter: blur(10px);
  backdrop-filter: blur(10px);
  border-radius: 10em;
}

.mockup-image {
  width: 20vw;
  height: 75vh;
}

article {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
@media only screen and (max-width:768px) {
  article{
    display: flex;
    flex-direction: column;
    justify-content: center;
  }
  #hero{
    display: flex;
    flex-direction: column;
    justify-content: center;
    margin-top: 5em;
  }
  #hero-image{
    width: 80vw;
  }
  .mockup-image{
    width: 80vw;
    height: 60vh;
  }
  .feature-background{
    width: 80vw;
  }
  .feature-text{
    margin: 1em 0;
  }
  section{
    margin: 2em 0;
    font-size: smaller;
  }
  .feature-image-content{
    margin-left: 0;
  }
}

.feature-description {
  margin: 0.5em 0;
  line-height: 2;
}

.feature-section {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.feature-icon {
  display: flex;
  align-items: center;
}

.feature-icon p {
  font-weight: 500;
}

.feature-tagline {
  font-weight: 600;
  text-decoration: underline;
}
</style>