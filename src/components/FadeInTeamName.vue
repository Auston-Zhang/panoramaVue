<template>
  <div class="fade-in-text">
  <p>Panorama FC</p>
  </div>
</template>

<script>

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
.fade-in-text {
  display: inline-block;
  font-family: Arial, Helvetica, sans-serif;
  font-size: 80px;
  color: whitesmoke;
  animation: fadeIn linear 5s;
  -webkit-animation: fadeIn linear 5s;
  -moz-animation: fadeIn linear 5s;
  -o-animation: fadeIn linear 5s;
  -ms-animation: fadeIn linear 5s;
  position: absolute;
  top:30%;
  left:30%;
}

@keyframes fadeIn {
  0% {opacity:0;}
  100% {opacity:1;}
}

@-moz-keyframes fadeIn {
  0% {opacity:0;}
  100% {opacity:1;}
}

@-webkit-keyframes fadeIn {
  0% {opacity:0;}
  100% {opacity:1;}
}

@-o-keyframes fadeIn {
  0% {opacity:0;}
  100% {opacity:1;}
}

@-ms-keyframes fadeIn {
  0% {opacity:0;}
  100% {opacity:1;}
}

</style>