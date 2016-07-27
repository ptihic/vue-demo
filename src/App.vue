<template>
  <div id="app">
    <title></title>
    <div class="article">
      <div class="list">
        <item></item>
      </div>
    </div>

  </div>
</template>

<script>
import Title from './components/title'
import Item from './components/item'

export default {
  components: {
    Title
  }
}
</script>

<style>
html {
  height: 100%;
}

body {
  display: flex;
  align-items:flex-start;
  justify-content:flex-start;
  height: 100%;
}

#app {
  color: #2c3e50;
  /*margin-top: -100px;*/
  max-width: 600px;
  font-family: Source Sans Pro, Helvetica, sans-serif;
  text-align: center;
}

#app a {
  color: #42b983;
  text-decoration: none;
}

.logo {
  width: 100px;
  height: 100px
}
</style>
