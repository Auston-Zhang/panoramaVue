<template>
  <div >
  <p class="fade-in-text">Panorama FC</p>
   <transition name="fade">
        <img class="container" v-bind:src="src" v-on:load="onLoaded" v-show="loaded">&nbsp;
   </transition>
  </div>
</template>

<script>
export default {
  name: 'LogoFadeIn',
  data: function() {
    return {
      src: require('../assets/Untitled-3.png'),
      loaded: false,
    }
  },
  methods: {
    onLoaded() {
    setTimeout(() => this.loaded = true, 3000);
      //this.loaded = true;
    }
  } 
}

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.fade-in-text {
  display: inline-block;
  font-family: Arial, Helvetica, sans-serif;
  font-size: 5rem;
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
.container {
  position: absolute;
  top:50%;
  left:10%;
  width: 100%;
  height:50%;
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

.fade-enter-active {
  transition: opacity 5s ease-in-out;
}
.fade-enter-to {
  opacity: 1;
}
.fade-enter {
  opacity: 0;
}



</style>