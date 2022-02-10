<template>
  <div id="nav">
    <Header />
    <AboutSection />
    <CheckSection />
    <RepresentSection />
  </div>
  <router-view/>
</template>

<script>
import Header from "@/components/Header";
import AboutSection from "@/components/AboutSection";
import CheckSection from "@/components/CheckSection";
import RepresentSection from "@/components/RepresentSection";

export default {
  components: {
    Header,
    AboutSection,
    CheckSection,
    RepresentSection,
  }
}
</script>
<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@100;400;600;700&display=swap');
#app {
  font-family: 'Montserrat', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

* {
  box-sizing: border-box;
}
li {
  list-style: none;
}
a {
  text-decoration: none;
  font-weight: 600;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 5px 15px;
}

#nav {
  a {
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
