<template>
<div class="menu">
  <div class="navigation-bar">
    <h1>
      <a class="hyperlink" href="/">Navigation Bar</a>
    </h1>
  </div>
  <div class="buger-bar">
  </div>  
</div>
</template>

<script>
export default {
  name: 'NavigationBar'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.menu {
  position: absolute;
  top: 3rem;
  width: 100%;
  background-color: transparent;
  height: 50px;
  z-index: 999;
}
.navigation-bar {
    padding-left: 90px;
    width: auto;
    float: left;
}
.buger-bar {
  position: absolute;
  top: 2.5rem;
  left: 0;
  height: 50px;
  z-index: 1002;
  transition: padding .2s ease-in-out;
}
.hyperlink {
  text-decoration: none;
  color: rgba(5,22,42,.87)
  
}
h1 {
  display: inline;
  text-align: left;
  letter-spacing: inherit;
    white-space: nowrap;
}
a {
  font-size: 2em;
  background-color: transparent;
  font-weight: 200;
}
a:hover {
  text-decoration: underline;
}
.buger-button {
  height: 50px;
}
.bar {
    top: 26px;
    transition: top .2s ease-in-out .1s,transform .2s ease-in-out .1s;
    animation: mrotl 2s cubic-bezier(.5,.2,.2,1.01);
}
</style>
