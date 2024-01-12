<template>
  <div class="body-background">
    <div class="container">
      <div id="view">
        <div id="view1">My</div>
        <div id="view2">Resume</div>
      </div>
      <div class="list" v-for="edu in education" :key="edu.id">
        <ul>
          <li>{{ edu.id }}</li>
          <li>{{ edu.year }}</li>
          <li>{{ edu.place }}</li>
          <li>{{ edu.type }}</li>
        </ul>
      </div>
      <div class="list2" v-for="any in skills" :key="any.id">
        <h2>{{ any.title }}</h2>
        <p>{{ any.experience }}</p>
      </div>
      <a
        class="btn btn-primary"
        target="_blank"
        href="https://docs.google.com/document/d/1Xttm3K48mRTXG54W3rzKmEe9kgQebRTW-m_kF_eirCk/edit?usp=sharing"
        role="button"
        >Resume</a
      >
    </div>
  </div>
</template>

<script>
export default {
  name: 'ResumeView',
  computed: {
    education() {
      return this.$store.state.education;
    },
    skills() {
      return this.$store.state.skills;
    },
  },
  mounted() {
    this.$store.dispatch('fetchData');
  },
};
</script>

<style scoped></style>
