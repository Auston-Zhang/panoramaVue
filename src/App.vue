<template>
  <div id="app">
    <b-navbar toggleable type="dark" variant="dark">
    <b-navbar-brand href="#">MENU</b-navbar-brand>

    <b-navbar-toggle target="navbar-toggle-collapse">
      <template #default="{ expanded }">
        <b-icon v-if="expanded" icon="chevron-bar-up"></b-icon>
        <b-icon v-else icon="chevron-bar-down"></b-icon>
      </template>
    </b-navbar-toggle>

    <b-collapse id="navbar-toggle-collapse" is-nav>
      <b-navbar-nav class="ml-auto">
        <b-nav-item href="#">Link 1</b-nav-item>
        <b-nav-item href="#">Link 2</b-nav-item>
        <b-nav-item href="#" disabled>Disabled</b-nav-item>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
  <HelloWorld/>
  <FadeInTeamName/>
  <Button/>
  </div>
  
        
</template>

<script>
import HelloWorld from './components/HelloWorld'
import Button from './components/Button'
import FadeInTeamName from './components/FadeInTeamName'


export default {
  name: 'App',
  components: {
    HelloWorld,
    Button,
    FadeInTeamName
  },
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 10px;
}

</style>
