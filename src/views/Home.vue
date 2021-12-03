<template>
  <div class="home">
    <div class="main">
      <div class="leftElm">
        <img src="../assets/call.png" class="call"/>
        <div class="objet">
        </div>
      </div>
      <div class="rightElm">
       <div class="content">
        <h1 class="headTtl">Enjoy your video call</h1>
        <div></div>
        <h4 class="center">with</h4>
        <div class="options center">
          <img src="../assets/v1.png" class="tall"/>
          <div class="spacer"></div>
          <img src="../assets/w1.png" class="tall">
        </div>
       </div>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src


export default {
  name: 'Home',
  components: {
    
  }
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,600;0,700;0,900;1,600&display=swap');

.center {
  display: flex;
  justify-content: center;
  align-items: center;
}

.tall {
  width: 130px;
  height: 130px;
}

.options {
  display: flex;
}
.spacer {
  margin: 0 20px 0 20px;
}

.main {
  width: 100%;
  display: flex;
  
}

.main .leftElm {
 width: 50%;
  height: 100vh;
  background-color: black;
  position: relative;
  border-radius: 0 50% 50% 0;
  background-image: url('../assets/blacl.jpeg');
}


.main .rightElm {
  width: 50%;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;

}

.wave2 {
  position: fixed;
  
  bottom: 0;
}

.call {
  animation: MoveUpDown 3s linear infinite;
  height: 500px;
  border-radius: 8px;
  position: absolute;
  top: 170px;
 left: 250px;
 right: 250px;
 
}

.headTtl {
 font-size: 100px;
 margin: 0 0 0 0;
 text-align: right;
 margin: 0 70px 90px 0;
 font-family: 'Montserrat';
 font-weight: 700;
 
}


.h4 {

  display: block;
}


@keyframes MoveUpDown {
  0%, 100% {
    transform: translateY(0);
  }
  50% {
    transform: translateY(-40px);
  }
}


@media screen and (max-width: 480px) {
  .main {
    display: block;
  }

  .main .leftElm {
    width: 100%;
    padding-bottom: 50px;
    border-radius: 0;
  }

  .wave1 {
    display: none;
  }
  .call {
    top: 70px;
    right: 0;
    left: 0;
    margin: 0 auto;
  }

  .headTtl {
    font-size: 30px;
    margin: 0;
    text-align: center;
    display: flex;
  justify-content: center;
  align-items: center;
  }


  .spacer{
   margin: 30px 0 0 0; 
  }

  .options {
    display: block;
  }

  .main .rightElm {
    margin: 0 auto;
  } 

}
</style>