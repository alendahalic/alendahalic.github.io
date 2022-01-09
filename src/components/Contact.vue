<template>
  <div class="contact" id="contact">
    <h2>Get in touch</h2>
    <hr>
    <p>I am only a click away!</p>
    <form action="https://formsubmit.co/49bdd57aa8cf7cece527849941ca2f49">
      <input type="text" name="name" placeholder="Full Name" required>
      <input type="email" name="email" placeholder="E-Mail Address" required>
      <textarea placeholder="Message" name="message" rows="10" columns="30" required></textarea>
      <button type="submit">Submit</button>
    </form>
  </div>
  <div id="scrollTop">
    <a href="#home">
      <svg width="30" height="18" viewBox="0 0 30 18" fill="none" xmlns="http://www.w3.org/2000/svg">
      <path d="M14.6464 5.30144L2.655 17.2929L0.707107 15.345L15 1.0521L29.2929 15.345L27.345 17.2929L15.3536 5.30144L15 4.94789L14.6464 5.30144Z" stroke="#efefef"/>
      </svg>
    </a>
    <p>Back to top?</p>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.contact{
  height: 90vh;
  padding-top: 200px;
  scroll-snap-align: start;
}
p{
  font-size: 14px;
  text-align: center;
}
hr{
  width: 350px;
  border-color: #fff;
  margin: auto;
  margin-top: 10px;
  margin-bottom: 10px;
}
h2{
    text-align: center;
    color: #fff;
}
form{
  margin-top: 50px;
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
  align-items: center;
  height: 400px;
  font-family: 'Inter', sans-serif;
}
input{
  width: 360px;
  border: transparent;
  padding: 10px;
  background: transparent;
  border-bottom: 1px solid #ff4444;
  color: #efefef;
}
button{
  transition: 100ms ease-in all;
  border: transparent;
  background: transparent;
  border: 1px solid #fff;
  width: 72px;
  padding: 10px;
  color: #fff;
  font-family: 'Inter', sans-serif;
  cursor: pointer;
}
button:hover{
  color: #121212;
  background: #fff;
}
textarea{
  width: 360px;
  background: transparent;
  border: 1px solid #ff4444;
  padding: 10px;
  color: #efefef;
  resize: none;
  font-family: 'Inter', sans-serif;
}
#scrollTop{
    height: 50px;
    width: 100px;
    display: flex;
    margin: auto;
    margin-top: 20px;
    margin-bottom: 20px;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
    font-size: 12px;
    color: #efefef;
}
@media screen and (max-width:475px) {
  .contact{
    padding-top: 100px;
  }
  form{
    margin-top: 20px;
  }
  input[type=text],input[type=email],textarea{
    width: 300px;
  }
  h2{
    margin:auto;
    font-size: 36px;
  }
  h2,hr{
    width: 300px;
  }
}

@media screen and (max-width:320px) {
  .contact{
    height: auto;
    padding-top: 50px;
  }
  form{
    height: 400px;
  }
}
</style>