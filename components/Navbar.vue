<template>
  <div>
    <b-navbar toggleable="sm">
      <div class="container">
        <b-navbar-brand>
          <nuxt-link to="/">ETIENNE P.</nuxt-link>
        </b-navbar-brand>
        <b-navbar-toggle target="nav-collapse">
          <img src="~/assets/img/menu-icon.png" alt="menu" width="22" />
        </b-navbar-toggle>
        <b-collapse id="nav-collapse" is-nav>
          <b-navbar-nav class="ml-auto">
            <b-nav-item class="home text-center">
              <nuxt-link to="/">HOME</nuxt-link>
            </b-nav-item>
            <b-nav-item-dropdown class="text-center" right text="WORK" toggle-class="nav-link-custom">
              <b-dropdown-item :to="'april'">AprilOn</b-dropdown-item>
              <b-dropdown-item :to="'ibubble'">iBubble</b-dropdown-item>
              <b-dropdown-item :to="'meet-your-beauty'">MeetYourBeauty</b-dropdown-item>
            </b-nav-item-dropdown>
            <b-nav-item class="text-center">
              <nuxt-link to="/">PROJECTS</nuxt-link>
            </b-nav-item>
            <b-nav-item class="text-center">
              <nuxt-link to="/">ABOUT</nuxt-link>
            </b-nav-item>
          </b-navbar-nav>
        </b-collapse>
      </div>
    </b-navbar>
  </div>
</template>
<style scoped lang="scss">
  .navbar {
    padding: 0.5rem 0rem;

    .container {
      font-family: 'Avenir Next', sans-serif;
      font-weight: 500;
      letter-spacing: 1px;
      color: #000000;
      cursor: pointer;
      font-size: 14px;
      padding-top: 40px;

      .navbar-toggler {
        border: none;
      }

      .navbar-brand {
        font-size: 16px;
        font-weight: 600;
        color: #191b1e;
      }

      a {
        color: #191b1e;
        text-decoration: none;

        &:hover {
          opacity: 0.8;
          color: #32343a;
        }
      }

      .navbar-nav {
        @media (min-width: 576px) {
          .nav-item {
            padding-right: 15px;

            &:last-child {
              padding-right: 0;
            }
          }
        }
      }
    }
  }
</style>
