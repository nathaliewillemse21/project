<template>
  <NavBar />
  <main class="container-fluid">
    <router-view />
  </main>
  <div>
  <SpinnerView />
  </div>
  <Footer />
</template>

<script>
import NavBar from './components/Navbar.vue';
import Footer from './components/Footer.vue';
import SpinnerView from './components/SpinnerView.vue';



export default {
  components: {
    NavBar,
    Footer,
    SpinnerView,
  },
};
</script>
<style src="@/assets/css/style.css"></style>
