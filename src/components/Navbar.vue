<template>
  <div>
        <b-navbar toggleable="lg" type="dark" variant="dark">
      <div class="container">
          <a href="https://bintoroarchitect.co.id">
           <img src="https://bintoroarchitect.co.id/media/LOGO%20NEW%20TEXT%20PUTIH-13%20200.webp">
           </a>
        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
        <b-collapse id="nav-collapse" is-nav>
          <b-navbar-nav>
            <li class="nav-item">
              <router-link class="nav-link" to="/">Home</router-link>
            </li>
            <li class="nav-item">
              <router-link class="nav-link" to="/">About</router-link>
            </li>
            <li class="nav-item">
              <router-link class="nav-link" to="/">Services</router-link>
            </li>
            <li class="nav-item">
              <router-link class="nav-link" to="/">Projects</router-link>
            </li>
            <li class="nav-item">
              <router-link class="nav-link" to="/">Blog</router-link>
            </li>
            <li class="nav-item">
              <router-link class="nav-link" to="/">Contact</router-link>
            </li>
          </b-navbar-nav>
        </b-collapse>
      </div>
    </b-navbar>
  </div>
</template>