<template>
  <div id="app">
    <!-- header -->
    <mainHeader />
    <!-- main conent -->
    <mainContent />
    <!-- section acquisti -->
    <mainSection />
    <!-- footer -->
    <mainFooter />
  </div>
</template>

<script>
import mainHeader from './components/MainHeader.vue';
import mainContent from './components/MainContent.vue';
import mainSection from './components/MainSection.vue';
import mainFooter from './components/MainFooter.vue';

export default {
  name: 'App',
  components: {
    mainHeader,
    mainContent,
    mainSection,
    mainFooter,
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
  width: 100%;
  height: 100%;
  display: block;
}

.container {
  max-width: 1300px;
  margin: 0 auto;
}

</style>
