<template>
  <div class="body-background">
    <div class="container">
      <div class="row">
        <div id="view">
          <div id="view1">Reach</div>
          <div id="view2">Me</div>
        </div>
      </div>
      <form action="https://formspree.io/f/mdoqovvq" method="POST">
        <div class="mb-3">
          <label for="exampleInputEmail1" class="form-label"
            >Email address</label
          >
          <input
            type="email"
            name="email"
            class="form-control"
            id="exampleInputEmail1"
            aria-describedby="emailHelp"
          />
        </div>
        <div class="mb-3">
          <label for="exampleInputContact1" class="form-label"
            >Contact Number</label
          >
          <input
            type="number"
            name="contact"
            class="form-control"
            id="exampleInputContact1"
          />
        </div>
        <div class="mb-3">
          <label for="exampleInputMessage1" class="form-label">Message</label>
          <textarea
            type="message"
            name="message"
            class="form-control"
            id="exampleFormControlTextarea1"
            rows="3"
          ></textarea>
        </div>
        <button type="submit" class="btn btn-primary m-3 p-1">Submit</button>
      </form>
      <img
        src="https://i.ibb.co/gjCdg24/Adobe-Stock-357056172.webp"
        class="img-fluid"
        alt="contact"
      />
    </div>
  </div>
</template>

<script>
export default {
  name: 'ContactView',
};
</script>

<style lang="stylus" scoped></style>
