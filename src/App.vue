<template>
  <div class="container">  
    <nav>
      <Header />
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </nav>
    <SidebarLeft />
    <SidebarRight />
  </div>
</template>

<script>
import Header from './components/Header'
import SidebarLeft from './components/SidebarLeft'
import SidebarRight from './components/SidebarRight'

export default {
  name: 'App',
  components: {
    Header,
    SidebarLeft,
    SidebarRight,
  },
  methods: {
  }
}
</script>

<style lang="scss">

body {
  background-color: grey;
  min-height: 100vh;
  margin: 0;

}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}


nav {
  display: flex; 
  align-items: center;
  justify-content: space-around;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
