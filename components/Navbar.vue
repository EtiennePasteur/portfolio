<template>
  <div>
    <b-navbar toggleable="sm">
      <div class="container">
        <b-navbar-brand>ETIENNE P.</b-navbar-brand>
        <b-navbar-toggle target="nav-collapse">
          <img src="~/assets/img/menu-icon.png" alt="menu" width="22" />
        </b-navbar-toggle>
        <b-collapse id="nav-collapse" is-nav>
          <b-navbar-nav class="ml-auto">
            <b-nav-item class="home text-center" href="#">HOME</b-nav-item>
            <b-nav-item-dropdown class="text-center" right text="WORK" toggle-class="nav-link-custom">
              <b-dropdown-item href="#">April</b-dropdown-item>
              <b-dropdown-item href="#">Neo9</b-dropdown-item>
              <b-dropdown-item href="#">Ubg</b-dropdown-item>
              <b-dropdown-item href="#">Sogilis</b-dropdown-item>
            </b-nav-item-dropdown>
            <b-nav-item-dropdown class="text-center" right text="PROJECTS" toggle-class="nav-link-custom">
              <b-dropdown-item href="#">April</b-dropdown-item>
              <b-dropdown-item href="#">Neo9</b-dropdown-item>
              <b-dropdown-item href="#">Ubg</b-dropdown-item>
              <b-dropdown-item href="#">Sogilis</b-dropdown-item>
            </b-nav-item-dropdown>
            <b-nav-item class="text-center" href="#">ABOUT</b-nav-item>
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
      font-family: Avenirnext, sans-serif;
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
        color: #000000;
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

        .home {
          font-weight: 600;

          .nav-link {
            color: #000000;

            &:hover {
              opacity: 0.8;
              color: #32343a;
            }
          }
        }
      }
    }
  }
</style>
