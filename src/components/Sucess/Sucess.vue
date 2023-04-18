<template>
  <div class="sucess">
    <div class="main-sucess">
      <div class="modal-sucess-header">
        <div class="thanks-image">
          <span class="thanks">
            <img id="icon" :src="icon_src" />
          </span>
        </div>
      </div>
      <div class="rate-result">
        <p>You selected {{ $root.rating }} out of 5</p>
      </div>
      <div class="modal-sucess-content">
        <h1>Thank you!</h1>
        <p>
          We appreciate you taking the time to giving a rating. If you ever need
          more support, dont hesitate to get in touch!
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Sucess",
  props: {
    selected: {
      type: Number,
      default: 0
    }
  },
  data() {
    return {
      icon_src: "/img/illustration-thank-you.svg",
      rating: null,
    };
  },
  created() {
    this.rating = this.$route.query.rating;
  },
};
</script>

<style src="./sucess.scss" lang="scss" scoped/>
