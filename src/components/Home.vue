<template>
  <div class="home" id="home">
    <div class="hero">
      <div class="bg-home"></div>
      <div class="content">
        <h1>Hello, <br> I am Alen</h1>
        <p>A web developer based in Bosnia and Herzegovina. 
        I enjoy making websites, and a bit of gaming in my spare time. I am fueled by creativity and coffee.</p>
      </div>
      <div class="bg-home"></div>
    </div>
    <div class="arrow">
      <a href="#work">
        <svg width="30" height="18" viewBox="0 0 30 18" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path d="M15.3536 13.0435L27.345 1.0521L29.2929 2.99999L15 17.2929L0.707107 2.99999L2.655 1.0521L14.6464 13.0435L15 13.3971L15.3536 13.0435Z" stroke="#fff"/>
        </svg>
      </a>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
h1{
  font-family: 'MADE Outer Sans', sans-serif;
  text-transform: uppercase;
  font-weight: 900;
  font-size: 72px;
  color: #fff;
  letter-spacing: 0.05em;
  border-bottom: 1px solid #ff4444;
  padding-bottom: 20px;
}
p{
  font-weight: 400;
  text-align: left;
  font-size: 14px;
  width: 250px;
  margin-top: 30px;
  margin-left: 250px;
}
.home{
  height: 100vh;
  margin: auto;
}
.arrow{
  width: 30px;
  margin: auto;
  cursor: pointer;
}
.hero{
  padding-top: 150px;
  display: flex;
  justify-content: space-evenly;
  align-items: center;
}
.bg-home{
  width: 300px;
  height: 700px;
  transition: 300ms ease all;
  background: url('../assets/bg_home.gif');
  filter: grayscale(1) brightness(2);
}
.bg-home:last-child{
  background: url('../assets/bg_home2.gif');
}
.bg-home:hover{
  filter: grayscale(0) brightness(1);
}
@media screen and (max-width:1156px) {
  .bg-home{
    display: none;
  }
}
@media screen and (max-width:475px){
  .home{
    width: 360px;
    padding-top: 40px;
  }
  nav{
    float: none;
    width: 300px;
    margin: auto;
  }
  h1{
    font-size: 56px;
  }
  p{
    text-align: left;
    margin-left: 50px;
  }
  .arrow{
    margin-top: 70px;
  }
}
@media screen and (max-width:360px){
  .home{
      width: 280px;
      padding-top: 0px;
  }
}
@media screen and (max-width:320px){
  h1{
    font-size: 56px;
  }
  .arrow{
    margin-top: 30px;
  }
}
</style>