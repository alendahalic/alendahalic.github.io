<template>
  <Nav/>
  <div class="cont">
    <Home/>
    <Work/>
    <Contact/>
    <div class="bg"></div>
  </div>
</template>

<script>
import Home from './components/Home.vue'
import Work from './components/Work.vue'
import Nav from './components/Nav.vue'
import Contact from './components/Contact.vue'

export default {
  name: 'App',
  components: {
    Home,
    Work,
    Contact,
    Nav
  }
}
</script>

<style>
@import url('https://fonts.cdnfonts.com/css/made-outer-sans-alt');
@import url('https://fonts.googleapis.com/css2?family=Inter&display=swap');

*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
.cont{
  max-width: 1280px;
  margin: auto;
}
html,body{
  scroll-behavior: smooth;
  scroll-snap-type: y proximity;
}
.bg{
    position: fixed;
    pointer-events: none;
    -webkit-animation: noise 1s steps(4) infinite;
    animation: noise 1s steps(4) infinite;
    background-image: url('assets/noise.png');
    height: 200%;
    left: -50%;
    top: -50%;
    width: 200%;
    opacity: 0.7;
    z-index: 99;
}
h2{
  font-family: 'MADE Outer Sans', sans-serif;
  text-align: center;
  font-size: 36px;
  color: #fff;
}
body{
  background: #000;
  color: #efefef;
  font-family: 'Inter', sans-serif;
}
@keyframes noise {
  0%{transform: translate(0, 0);}
  10%{transform: translate(-5%, -5%);}
  20%{transform: translate(-10%, 5%);}
  30%{transform: translate(5%, -10%);}
  40%{transform: translate(-5%, 15%);}
  50%{transform: translate(-10%, 5%);}
  60%{transform: translate(15%, 0);}
  70%{transform: translate(0, 10%);}
  80%{transform: translate(-15%, 0);}
  90%{transform: translate(10%, 5%);}
  100%{transform: translate(5%, 0);}
}
</style>
