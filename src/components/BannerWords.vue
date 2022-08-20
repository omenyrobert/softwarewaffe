<template>
  <div id="app">
    <div class="row">
      <div class="col-md-2">
        <div id="carouselExampleSlidesOnly" class="carousel slide" data-bs-ride="carousel">
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img style="width: 100%; margin-top: 50px;"
          src="https://res.cloudinary.com/dtlkiv19d/image/upload/v1660980050/Kallery/sw/sw23-min_gfvb3a.png"
        />
        <img
        style="width: 100%; margin-top: 50px;"
          src="https://res.cloudinary.com/dtlkiv19d/image/upload/v1660979796/Kallery/sw/sw25_p32phe.png"
        />
    </div>
    <div class="carousel-item">
      <img style="width: 100%; margin-top: 50px;"
          src="https://res.cloudinary.com/dtlkiv19d/image/upload/v1660980050/Kallery/sw/sw23-min_gfvb3a.png"
        />
        <img
        style="width: 100%; margin-top: 50px;"
          src="https://res.cloudinary.com/dtlkiv19d/image/upload/v1660979796/Kallery/sw/sw25_p32phe.png"
        />
    </div>
    <div class="carousel-item">
      <img style="width: 100%; margin-top: 50px;"
          src="https://res.cloudinary.com/dtlkiv19d/image/upload/v1660980050/Kallery/sw/sw23-min_gfvb3a.png"
        />
        <img
        style="width: 100%; margin-top: 50px;"
          src="https://res.cloudinary.com/dtlkiv19d/image/upload/v1660979796/Kallery/sw/sw25_p32phe.png"
        />
    </div>
  </div>
</div>

      </div>
      <div class="col-md-8">
         <div class="wrapper">
    <div class="static-txt">I'm a</div>
    <ul class="dynamic-txts">
      <li><span>YouTuber</span></li>
      <li><span>Designer</span></li>
      <li><span>Developer</span></li>
      <li><span>Freelancer</span></li>
    </ul>
  </div>
      </div>
      <div class="col-md-2 pl-5">
        <div id="carouselExampleSlidesOnly" class="carousel slide" data-bs-ride="carousel">
  <div class="carousel-inner">
    <div class="carousel-item active">
   <img
        style="width: 70%; margin-top: 50px;"
          src="https://res.cloudinary.com/dtlkiv19d/image/upload/v1660913419/Kallery/sw/sw3_ra35ia.png"
        />
         <img
        style="width: 70%; margin-top: 20px;"
          src="https://res.cloudinary.com/dtlkiv19d/image/upload/v1660913889/Kallery/sw/sw14_uvfytv.png">
    </div>
    <div class="carousel-item">
   <img
        style="width: 70%; margin-top: 50px;"
          src="https://res.cloudinary.com/dtlkiv19d/image/upload/v1660913419/Kallery/sw/sw3_ra35ia.png"
        />
         <img
        style="width: 70%; margin-top: 20px;"
          src="https://res.cloudinary.com/dtlkiv19d/image/upload/v1660913889/Kallery/sw/sw14_uvfytv.png">
    </div>
    <div class="carousel-item">
   <img
        style="width: 70%; margin-top: 50px;"
          src="https://res.cloudinary.com/dtlkiv19d/image/upload/v1660913419/Kallery/sw/sw3_ra35ia.png"
        />
         <img
        style="width: 70%; margin-top: 20px;"
          src="https://res.cloudinary.com/dtlkiv19d/image/upload/v1660913889/Kallery/sw/sw14_uvfytv.png">
    </div>
  </div>
</div>
        

        
        
      </div>
    </div>
  </div>
</template>

<script>


export default {
  name: "App",
  components: {

  },
  data (){
   return {

   }
  },
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@200;300;400;500;600;700&display=swap');
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Poppins', sans-serif;
}
.wrapper{
  display: flex;
}
.wrapper .static-txt{
  color: #fff;
  font-size: 60px;
  font-weight: 400;
}
.wrapper .dynamic-txts{
  margin-left: 15px;
  height: 90px;
  line-height: 90px;
  overflow: hidden;
}
.dynamic-txts li{
  list-style: none;
  color: #FC6D6D;
  font-size: 60px;
  font-weight: 500;
  position: relative;
  top: 0;
  animation: slide 12s steps(4) infinite;
}
@keyframes slide {
  100%{
    top: -360px;
  }
}
.dynamic-txts li span{
  position: relative;
  margin: 5px 0;
  line-height: 90px;
}
.dynamic-txts li span::after{
  content: "";
  position: absolute;
  left: 0;
  height: 100%;
  width: 100%;
  background: #ffffff;
  border-left: 2px solid #FC6D6D;
  animation: typing 3s steps(10) infinite;
}
@keyframes typing {
  40%, 60%{
    left: calc(100% + 30px);
  }
  100%{
    left: 0;
  }
}
</style>