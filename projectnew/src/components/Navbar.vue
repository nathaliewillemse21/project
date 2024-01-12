<template>
  <nav class="navbar navbar-expand-lg">
    <div class="container-fluid">
      <router-link to="/">
        <img
          class="img-fluid"
          src="https://i.ibb.co/tbQynkf/NW.png"
          loading="lazy"
          alt="logo"
        />
      </router-link>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <router-link to="/" class="nav-link active">Home | </router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/about">About | </router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/resume">Resume | </router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/testimonials"
              >Testimonials |
            </router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/project">Project | </router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/contact">Contact | </router-link>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'NavBar',
};
</script>

<style scoped></style>
