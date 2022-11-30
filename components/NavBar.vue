<template>
  <div>
    <vs-navbar
      v-model="activeItem"
      :class="
        $route.name === 'about'
          ? 'about'
          : $route.name === 'contact'
          ? 'contact'
          : ''
      "
      class="nabarx"
    >
      <div slot="title">
        <vs-navbar-title>
          <img alt="" class="nav-logo" src="/icon.png" />
        </vs-navbar-title>
      </div>

      <vs-navbar-item index="0">
        <nuxt-link to="/">Home</nuxt-link>
      </vs-navbar-item>
      <vs-navbar-item index="1">
        <nuxt-link to="/about">About</nuxt-link>
      </vs-navbar-item>
      <vs-navbar-item index="2">
        <nuxt-link to="/contact">Contact</nuxt-link>
      </vs-navbar-item>
    </vs-navbar>
  </div>
</template>

<script>
export default {
  name: 'NavBar',
  data() {
    return {
      activeItem: 0,
    }
  },
}
</script>

<style lang="scss">
.uk-sticky.uk-sticky-below {
  background: #fafafa;

  .vs-navbar--item {
    a {
      color: #0a0a0a;
      font-size: 1rem;
    }
  }
}

.vs-navbar {
  padding: 0 5%;
  min-height: 80px;
  position: absolute;

  .nav-logo {
    height: 60px;
  }

  &.about {
    .vs-navbar--item {
      a {
        color: #0a0a0a;
        font-size: 1rem;
      }
    }
  }

  .vs-navbar--item {
    a {
      color: #fafafa;
      font-size: 1rem;
    }
  }
}

.uk-sticky {
  position: absolute;
  width: 100%;
}

.uk-sticky-placeholder {
  position: absolute;
}
</style>
