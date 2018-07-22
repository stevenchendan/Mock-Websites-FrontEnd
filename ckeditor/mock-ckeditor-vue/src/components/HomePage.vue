<template>
<section>
  <video class="home-page-video" 
    muted="" autoplay="" loop="" 
    data-src="../assets/video/home-bg.mp4" 
    src="../assets/video/home-bg.mp4"></video>
  <div class="home-page-title">
    <h1>Steven Mock ckeditor</h1>
    <h2>
      I like the design of the front page. I use vue framework to
      mock the design of this website.
    </h2>
  </div>
  <span class="scroll-down-icon">
    <svg width="34" height="57">
      <g fill="none" fill-rule="evenodd">
        <rect stroke="#000" stroke-width="2" x="1" y="1" width="32" height="54.667" rx="15"></rect>
        <circle id="mouse-scroll" fill="#000" cx="17" cy="14.481" r="3.148"></circle>
      </g>
    </svg>
  </span>
</section>
  
</template>

<script>
export default {
  name: 'HomePage',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
h1 {
  font-size: 5.4rem;
  font-weight:600;
  margin-top: 0;
  margin-bottom: 0;
  line-height: 7.5rem;
}
h2 {
  font-size: 3.5rem;
  font-weight: 200;
  line-height: 4rem;
  margin-top: 0;
  width: 880px;
  margin: 1.25rem auto 0;
}
.home-page-title {
  position: absolute;
  top: 50%;
  left: 50%;
  width: 90%;
  text-align: center;
  transform: translate(-50%,-50%);
  z-index: 9;
}
section:before {
  width: 490px;
  height: 517px;
  margin-top: -180px;
  content: '';
    display: block;
    position: absolute;
    top: 50%;
    left: 50%;
    width: 350px;
    height: 360px;
    margin-top: -150px;
    background-image: url(../assets/images/home/logo-ecosystem-3caa270218.svg);
    background-repeat: no-repeat;
    background-position: center top;
    background-size: contain;
    transform: translate(-50%,-50%);
    z-index: 2;
}
.scroll-down-icon {
    display: block;
    position: absolute;
    left: 50%;
    bottom: 5rem;
    width: 35px;
    height: 57px;
    opacity: .7;
    z-index: 10;
    transform: translateX(-50%);
    transition: opacity .2s ease-in-out;
}
.home-page-video {
    display: block;
    position: absolute;
    /* opacity: 0; */
    min-height: 100%;
    min-width: 100%;
    top: 0px;
    left: 0px;
}
.home-page-video::after {
  background-image: url(../assets/images/home/video-mask.svg);
}
</style>
