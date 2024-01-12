<template>
  <div>
    <div class="d-flex justify-content-center">
      <div class="spinner-border" v-if="isLoading" role="status">
        <span class="visually-hidden">Loading...</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SpinnerView',
  data() {
    return {
      loading: true,
    };
  },
  method: {
    fetchData() {
      this.isloading = true;
      setTimeout(() => {
        this.isLoading = false;
      }, 2000);
    },
  },
};
</script>

<style scoped></style>
