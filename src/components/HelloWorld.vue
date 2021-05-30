<template>
   <div class="container">
      <transition name="fade">
        <img class="container" v-bind:src="src" v-on:load="onLoaded" v-show="loaded">&nbsp;
      </transition>
   </div>
</template>

<script>
// https://stackoverflow.com/questions/47535317/how-to-fade-in-images-when-loaded-with-vue
export default {
  name: 'HelloWorld',
  data: function() {
    return {
      src: require('../assets/backgroundSmall.jpeg'),
      loaded: false,
    }
  },
  methods: {
    onLoaded() {
      this.loaded = true;
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.container {
  min-width: 100%;
  max-height: 100%;
  background: black;
}

h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
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
