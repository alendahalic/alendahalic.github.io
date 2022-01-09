<template>
  <nav>
    <a href="#work">portfolio</a>
    <a href="">resume</a>
    <a href="#contact">contact</a>
  </nav>
</template>

<script>
export default {

}
</script>

<style>
nav{
  position: fixed;
  top: 0;
  width: 100vw;
  height: 100px;
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  z-index: 999;
  backdrop-filter: blur(4px);
  background: rgba(0, 0, 0, .7);
}
nav a{
  font-family: 'MADE Outer Sans', sans-serif;
  transition: 200ms ease-in-out all;
  color: #efefef;
  text-decoration: none;
  font-size: 18px;
  padding: 10px;
  font-weight: 400;
  border: 2px solid transparent;
}
nav a:hover,nav a:active{
  color: #ff4444;
  border-bottom-color: #ff4444;
}
</style>