<template>
  <div class="home">
    <div class="main">
      <div class="modal-header">
        <div class="star-image">
          <span class="star">
            <img id="icon" :src="icon_src">
          </span>
        </div>
      </div>
      <div class="modal-content">
        <h1>How did we do?</h1>
        <p>
          Please let us know how we did with your support request. All feedback
          is appreciated to help us improve our offering!
        </p>
      </div>
      <div class="rate-options">
        <div class="rate">
          <ul>
            <li id="1" v-on:click="select($event)">
              <a>1</a>
            </li>
            <li id="2" v-on:click="select($event)">
              <a>2</a>
            </li>
            <li id="3" v-on:click="select($event)">
              <a>3</a>
            </li>
            <li id="4" v-on:click="select($event)">
              <a>4</a>
            </li>
            <li id="5" v-on:click="select($event)">
              <a>5</a>
            </li>
          </ul>
        </div>
      </div>
      <router-link to="/sucess">
        <button id="btn">
          <span>Submit</span>
        </button>
      </router-link>
    </div>
  </div>
</template>
<script>
export default {
  name: "Rating",

  data() {
    return {
      icon_src: ('/img/icon-star.svg'),
    }
  },
  methods: {
    select: function(event) {
      let targetId = event.currentTarget.id;
    }
  }
}
</script>

<style src="./rating.scss" lang="scss" scoped/>