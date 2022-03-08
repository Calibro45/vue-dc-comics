<template>
  <div id="app">
    <!-- header -->
    <mainHeader />
    <!-- main conent -->
    <!-- section acquisti -->
    <!-- footer -->
  </div>
</template>

<script>
import mainHeader from './components/MainHeader.vue';
//import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    mainHeader,

  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;500;700&display=swap');

* {
  margin: 0;
  padding: 0;
  box-sizing:  border-box;
}

html {
  font-size: 16px;
  font-family: 'Roboto', sans-serif;
}

ol, ul {
  list-style-type: none;
}

a {
  text-decoration: none;
  color: currentColor;
}

img {
  max-width: 100%;
  height: 100%;
}

.container-fluid {
  width: 100%;
}

.container {
  max-width: 1300px;
  margin: 0 auto;
}

</style>
