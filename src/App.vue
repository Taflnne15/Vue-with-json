<template>
  <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
  </nav>
  <router-view/>
 <Footer/>
</template>
<script>
import Footer from '@/components/Footer.vue';

  export default {
    components: {
      Footer,
    }
  }
</script>



<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
.card-body{
  border: solid black 4px;
  background-color: #42b983;
}
h6{
  font-weight: 600;
}
</style>
