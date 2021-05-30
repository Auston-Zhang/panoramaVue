<template>
  <button class='btn btn-dark' size = "lg"> Continue>> </button>
</template>

<script>

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>

.btn{
  animation: blinker 2s linear infinite;
  position: absolute;
  border:5px;
  border-color: white;
  top:100%;
  left:45%;
}


@keyframes blinker {
  50% {
    opacity: 0.5;
  }
}

</style>
