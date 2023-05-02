<script setup></script>
<template>


  <!-- <video autoplay muted loop id="bgVideo">

    <source src="../assets/dining.mp4" type="video/mp4" />
    
    Your browser does not support HTML5 video.
  </video> -->

  <div class="bg-image">
    <p>
      <!-- This is a paragraph of text. -->

    </p>
  </div>

  
</template>
<style scoped>
/* p {
  background-image: url('../assets/bg.png');
} */
.bg-image{
  height: 100vh;
  width: 100%;
  background-image: url('../assets/bg.png');
  background-size: cover;
  padding: 20px;
}


  

video {
  height: 100vh;
  width: 100%;
  object-fit: fill;
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
