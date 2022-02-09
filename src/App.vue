<template>
  <div id="nav">
    <Header />
    <Introduce />
    <CheckSection />
  </div>
  <router-view/>
</template>

<script>
import Header from "@/components/Header";
import Introduce from "@/components/Introduce";
import CheckSection from "@/components/CheckSection";

export default {
  components: {
    Header,
    Introduce,
    CheckSection,
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
