<template>
  <section class="production-section">
    <div class="production-card production-editor-5">
      <h3>Editor 5</h3>
      <p>Lorem ipsum dolor sit amet, mei quas sententiae ut. 
        Vel exerci possim deleniti ad. Ex nam</p>
        <a class="" href="">
        Learn more</a>
    </div>
    <div class="production-card production-editor-4">
      <h3>Editor 4</h3>
      <p>Lorem ipsum dolor sit amet, mei quas sententiae ut. 
        Vel exerci possim deleniti ad. Ex nam</p>
        <a class="" href="">
        Learn more</a>
    </div>
    <div class="production-card production-cloud-service">
      <a class="" href="">
        <h3>Editor Cloud Service</h3>
        <p>Lorem ipsum dolor sit amet, mei quas sententiae ut. 
          Vel exerci possim deleniti ad. Ex nam</p>
        <span class="btn">Learn more</span>
      </a>
    </div>
  </section>
</template>

<script>
export default {
  name: 'ProductionPage'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.production-section {
  display: inline-flex;
  margin-top: 110vh;
  margin-left: auto;
  margin-right: auto;
  width: 100%;
  height: 30vh;
  max-width: none;
}
.btn {
  color: #fff;
  border-color: #2e9fff;
  background-color: #2e9fff;
}

.production-card {
  position: relative;
  text-align: center;
  overflow: hidden;
  border-radius: 4px;
  transition: all .2s ease-in-out;
  margin-right: 5%;
}
.production-card::after {
    content: '';
    position: absolute;
    top: 2.5rem;
    left: 50%;
    width: 104px;
    height: 97px;
    margin-left: 8px;
    background-repeat: no-repeat;
    background-size: contain;
    background-position: center top;
    transform: translate3d(-50%,0,0);
    z-index: 3;
}
.production-editor-5 {

  margin-left: 19%;
}
.production-editor-5::after {
    background-image: url(../assets/images/product/icon-ckeditor-5.svg);
}
.production-editor-4::after {
    background-image: url(../assets/images/product/icon-ckeditor-4.svg);
}
.production-cloud-service::after {
    background-image: url(../assets/images/product/icon-cloud.svg);
}
</style>
