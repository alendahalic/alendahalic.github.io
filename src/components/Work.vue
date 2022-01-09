<template>
  <div class="work" id="work">
      <header>
        <div class="h2">
            <h2>My Work</h2>
        </div>
        <div class="img" style="width:32px;">
          <svg width="32" height="32" viewBox="0 0 32 32" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M18.0143 20.1353L1.12665 3.24764L3.25293 1.12135L20.1406 18.009L20.993 18.8615L20.9941 17.6559L21.0078 2.33094L24.0034 2.33094L24.0034 23.9981L2.33624 23.9981L2.33624 21.0025L17.6612 20.9888L18.8668 20.9877L18.0143 20.1353Z" stroke="#efefef"/>
          </svg>
        </div>
      </header>
      <section>
          <div class="frame"></div>
          <div class="frame"></div>
          <div class="frame"></div>
      </section>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.work{
    height: 100vh;
    padding-top: 100px;
    scroll-snap-align: start;
}
header{
    display: flex;
    width: 250px;
    height: 80px;
    justify-content: space-between;
    align-items: center;
    border-bottom: 1px solid #ff4444;
}
section{
    padding-top: 100px;
    display: flex;
    justify-content: space-evenly;
    align-items: center;
}
.frame{
    transition: 200ms all ease-in-out;
    width: 350px;
    height: 500px;
    padding: 20px;
    background: #efefef;
    color: #121212;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-evenly;
}
.frame:hover{
    transform: scale(1.1);
}
p{
  font-size: 14px;
  width: 200px;
  margin: auto;
}
@media screen and (max-width:1024px){
  section{
    flex-direction: column;
  }
  .work{
    height: auto;
  }
  .frame{
    width: 600px;
    height: 450px;
    margin: 20px 0px;
    padding: 20px;
  }
  header{
    margin: auto;
  }
  header .img{
    transform: rotateZ(90deg);
  }
}
@media screen and (max-width:475px) {
  .work{
    padding-top: 100px;
  }
  section{
    padding-top: 20px;
  }
  .frame{
    width: 300px;
    height: 360px;
    margin: 20px 0px;
    padding: 20px;
  }
}

@media screen and (max-width:320px) {
  .frame{
    width: 280px;
  }
}
</style>