<template>
  <div>
    <b-navbar toggleable="sm" type="light" variant="light">
      <div class="container">
        <b-navbar-brand>ETIENNE PASTEUR</b-navbar-brand>
        <b-collapse id="nav-collapse" is-nav>
          <b-navbar-nav class="ml-auto">
            <b-nav-item href="#">HOME</b-nav-item>
            <b-nav-item-dropdown text="WORK" right>
              <b-dropdown-item href="#">April</b-dropdown-item>
              <b-dropdown-item href="#">Neo9</b-dropdown-item>
              <b-dropdown-item href="#">Ubg</b-dropdown-item>
              <b-dropdown-item href="#">Sogilis</b-dropdown-item>
            </b-nav-item-dropdown>
            <b-nav-item-dropdown text="PROJECTS" right>
              <b-dropdown-item href="#">April</b-dropdown-item>
              <b-dropdown-item href="#">Neo9</b-dropdown-item>
              <b-dropdown-item href="#">Ubg</b-dropdown-item>
              <b-dropdown-item href="#">Sogilis</b-dropdown-item>
            </b-nav-item-dropdown>
            <b-nav-item href="#">ABOUT</b-nav-item>
          </b-navbar-nav>
        </b-collapse>
        <b-navbar-toggle target="nav-collapse" />
      </div>
    </b-navbar>
  </div>
</template>
