<template>
  <main class="home--section">
    <section class="page">
      <div class="container">
        <div class="header--text">
          <h3>Bringing Utility to Live</h3>
          <p>We believe in a future with abundant opportunities and prosperity for all and the role of technology
            towards achieving this future.</p>
          <div class="action--buttons">
            <nuxt-link class="btn btn--theme" to="/about">Learn More</nuxt-link>
            <nuxt-link class="btn btn--color" to="/contact">Contact Us</nuxt-link>
          </div>
        </div>
        <div class="header--img">
          <img alt="" src="/header-pic.png">
        </div>
      </div>
    </section>
    <section class="container what-we-do">
      <h3 class="uk-text-center">What We Do</h3>
      <div class="grid-col-3">
        <div class="what">
          <img alt="" src="/what1.png"/>
          <div class="what--content">
            <h5>Bringing Utility to Live</h5>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aliquid dolorum enim et hic ipsa iusto laborum
              officia repellat suscipit voluptatibus?</p>
          </div>
        </div>
        <div class="what">
          <img alt="" src="/what2.png"/>
          <div class="what--content">
            <h5>Bringing Utility to Live</h5>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aliquid dolorum enim et hic ipsa iusto laborum
              officia repellat suscipit voluptatibus?</p>
          </div>
        </div>
        <div class="what">
          <img alt="" src="/what3.png"/>
          <div class="what--content">
            <h5>Bringing Utility to Live</h5>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aliquid dolorum enim et hic ipsa iusto laborum
              officia repellat suscipit voluptatibus?</p>
          </div>
        </div>
      </div>
    </section>
    <section class="container transform">
      <div class="trans--img">
        <img alt="" src="/transform-img.png">
      </div>
      <div class="trans--text">
        <h4>Transforming Web3 ideas. Digitally.</h4>
        <p>Lorem ipsum dolor sit amet consectetur. Sed amet amet vulputate netus ornare pretium in. Id ultricies diam
          facilisis ut lacinia. Ut ornare amet vitae Lorem ipsum dolor sit amet consectetur. Sed amet amet vulputate
          netus ornare pretium in. Id ultricies diam facilisis ut lacinia. Ut ornare amet vitae </p>
        <a class="btn btn--theme" href="#">Start a Project</a>
      </div>
    </section>
    <section class="explore">
      <div class="container">
        <div class="explore--text">
          <h4>Explore Nifitiqet, Our Product</h4>
          <p>Lorem ipsum dolor sit amet consectetur. Sed amet amet vulputate netus ornare pretium in. Id ultricies diam
            facilisis ut lacinia. Ut ornare amet vitae Lorem ipsum dolor sit amet consectetur. Sed amet amet vulputate
            netus ornare pretium in. Id ultricies diam facilisis ut lacinia. Ut ornare amet vitae</p>
          <a class="btn btn--theme" href="#">Explore</a>
        </div>
        <div class="explore--img">
          <img alt="" src="/explore-img.png">
        </div>
      </div>
    </section>
  </main>
</template>

<script>
export default {
  name: 'IndexPage',
}
</script>
