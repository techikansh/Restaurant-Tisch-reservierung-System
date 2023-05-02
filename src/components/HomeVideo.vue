<script setup></script>
<template>


  <video autoplay muted loop id="bgVideo">

    <source src="../assets/bg_video.mp4" type="video/mp4" />
    
    Your browser does not support HTML5 video.
  </video>


  <!-- written by dev for background image -->

  <div class="bg-image">
    <p>
      <!-- This is a paragraph of text. -->

    </p>
  </div>

  
</template>
<style scoped>

/* written by dev for background image  */
/* 
.bg-image{
  height: 100vh;
  width: 100%;
  background-image: url('../assets/bg.png');
  background-size: cover;
  padding: 20px;
} */


  

video {
  height: 100vh;
  width: 100%;
  object-fit: fill;
  filter : contrast(200%);
  filter : blur(8px);
  animation: 1.2s ease-out 0s 1 slideUp;
}

@keyframes slideUp {
  0% {
    transform: translateY(20vh);
  }
  100% {
    transform: translateY(0);
  }
}
</style>
