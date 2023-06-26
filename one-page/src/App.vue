<template>
  <nav class="nav">
    <img src="https://i.postimg.cc/hG8Yh8mB/a94b35b2008b44f9727eac9ad5fa5b96.jpg" alt="" class="logo">
    <router-link to="/">Home</router-link> 
    
  </nav>
  <router-view/>
  <Footer />
</template>
<script>
import Footer from './components/footer.vue';

export default{
  components:{
    Footer
  }
}
</script>
<style>
.logo{
  height: 3rem;
  display: flex;
  align-content: start;
  
}
.nav{
  background-color: black;
}
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
  color: #f0f0f0;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
