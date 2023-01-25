<template>
  <div class="home">
    <div class="main">
      <div class="modal-header">
        <div class="star-image">
          <span class="star">
            <img src="images/icon-star.svg" alt="star-image" />
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
            <li>
              <a id="1" onClick="getRate(this.id)">1</a>
            </li>
            <li>
              <a id="2" onClick="getRate(this.id)">2</a>
            </li>
            <li>
              <a id="3" onClick="getRate(this.id)">3</a>
            </li>
            <li>
              <a id="4" onClick="getRate(this.id)">4</a>
            </li>
            <li>
              <a id="5" onClick="getRate(this.id)">5</a>
            </li>
          </ul>
        </div>
      </div>
      <button id="btn">
        <router-link to="/sucess">Submit</router-link>
      </button>
    </div>
  </div>
</template>
<script>
export default {
  name: "Home",
}
</script>

<style src="./style.scss" lang="scss" scoped/>