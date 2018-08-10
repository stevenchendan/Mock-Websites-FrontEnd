<template>
  <section class="production-section">
    <div class="production-card production-editor-5">
      <h3>Editor 5</h3>
      <p >Lorem ipsum dolor sit amet, mei quas sententiae ut. 
        Vel exerci possim deleniti ad. Ex nam</p>
        <span class="learn-more btn" href="">
        Learn more</span>
    </div>
    <div class="production-card production-editor-4">
      <h3>Editor 4</h3>
      <p>Lorem ipsum dolor sit amet, mei quas sententiae ut. 
        Vel exerci possim deleniti ad. Ex nam</p>
        <span class="learn-more btn" href="">
        Learn more</span>
    </div>
    <div class="production-card production-cloud-service">
        <h3>Editor Cloud Service</h3>
        <p>Lorem ipsum dolor sit amet, mei quas sententiae ut. 
          Vel exerci possim deleniti ad. Ex nam</p>
        <span class="learn-more btn">Learn more</span>
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
  height: 35vh;
  max-width: none;
  margin-bottom: 10%;
}
.btn {
  color: #fff;
  border-width: 1px;
  background-color: #fff;
  border: 2px solid #979797;
  border-radius: 4px;
}

.production-card {
  position: relative;
  text-align: center;
  border-radius: 4px;
  transition: all .2s ease-in-out;
  margin-right: 5%;
  width: 330px;
}

.production-card:hover {
    box-shadow: 1px 8px 20px grey;
    -webkit-transition:  box-shadow .6s ease-in;
}


.production-card p {
  font-size: 2rem;
  max-width: 100%;
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
h3 {
  padding-top: 20vh;
  font-size: 3rem;
}
.learn-more {
    border-color: #979797;
    color: rgba(5,22,42,.87);
    background-color: #fff;
    border: 2px solid #979797;
    border-width: 1px;
    min-width: 17.5rem;
    padding: 10px 50px;
    font-size: 1.6rem;
    min-height: 10vh;
}

.btn:hover {
    background-color: #007ac9 !important;
    border: 2px solid #007ac9 !important;
    cursor: pointer;
    
}

</style>
