<template>
  <div class="body-background">
    <div class="container">
      <div id="view">
        <div id="view1">My</div>
        <div id="view2">Testimonials</div>
      </div>
      <div class="card mb-3" v-for="test in testimonials" :key="test.id">
        <div class="row g-0">
          <div class="col-md-4">
            <img
              :src="test.profile"
              class="card-img-top w-50"
              loading="lazy"
              alt="Testimonial Image"
            />
          </div>

          <div class="col-md-8">
            <div class="card-body">
              <h5 class="card-title">{{ test.name }} {{ test.surname }}</h5>
              <p class="card-text">"{{ test.quotes }}"</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'TestimonialsView',
  computed: {
    testimonials() {
      return this.$store.state.testimonials;
    },
  },
  mounted() {
    this.$store.dispatch('fetchData');
  },
};
</script>

<style scoped></style>
