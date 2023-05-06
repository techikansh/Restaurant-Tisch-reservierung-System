<script setup>
const bgVideo = document.getElementById('bgVideo')

function test() {
  bgVideo.style.display = 'none'
  console.log(bgVideo)
}

function scrollToContent(){
  var contentElement = document.getElementById("content1");
  contentElement.scrollIntoView({behavior : "smooth"});
}

</script>
<template>
  <div class="d-flex flex-column text-center justify-content-between" id="videoContent">
    <div class="">
      <img src="../assets/los.svg" id="logoWrapper" height="350" width="350" alt="" />
      
      <div class = "reserve-you-table" id = "r-y-t">
        <!-- <p>Reserve you Table</p> -->
      </div>

      <div class="mt-5" id="reserve">
        <router-link class="nav-link" id="reserveBtn" :to="{ name: 'reservieren' }"
          >Reserve Now!</router-link>
      </div>
    </div>

    <div class="mb-4" id="scroll">
      <span id="scroll_link" >
        Esplorare
        <img src="../assets/icons/arrow_down.png" class="mt-3" id="arrow" alt="" />
      </span>
    </div>
  </div>
</template>
<style scoped>

#r-y-t{
  color : #F8B333;
  font-size: 90px;
  font-family: 'Chalkduster', bold;
  transform: translate(0%, 435%);

}

#videoContent {
  min-height: calc(100vh - 150px);
  padding-top: 15rem;
}
#logoWrapper {
  /* margin: 20vh 0 0 35px; */
  border-radius: 50% 50%;
}


#reserveBtn {
  /* transform: translate(0%, 1035%); */
  color: #fff;
  display: inline-block;
  /* display : flex; */
  align-items: center;
  font-size: 33px;
  font-weight: 2000;
  font-family: 'BoucherieCursive', Bold, cursive;
  line-height: 46px;
  letter-spacing: calc(100px / 100);
  border: 2px solid #fff;
  border-radius: 50px;
  padding: 1px 45px 5px 45px;
  transition: 0.3s;
  opacity: 0.8;
}
#reserveBtn:hover {
  font-weight: 200;
  background-color: #fff;
  color: #F8B333;
  opacity: 1;
}
#scroll {
  text-align: center;
  cursor: pointer;
  /* opacity: 0.3; */
}
#scroll_link {
  color: #fff;
  font-size: 1.625rem;
  font-family: 'BoucherieCursive', cursive;
  display: flex;
  flex-direction: column;
  align-items: center;
}
#arrow {
  height: 25px;
  width: 25px;
}
</style>

<script>

  function scrollToContent(){
  var contentElement = document.getElementById("menu-font");
  contentElement.scrollIntoView({behavior : "smooth"});
}

</script>




