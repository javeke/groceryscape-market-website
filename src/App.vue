<template>
  <div id="app">
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
      <div class="container-fluid">
        <a class="navbar-brand" href="/">
          <img src="./assets/default.svg" alt="GroceryScape" width="100" height="100">
        </a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav me-auto mb-2 mb-lg-0">
            <li class="nav-item">
              <router-link class="nav-link active" to="/">Home</router-link> 
            </li>
            <li class="nav-item">
              <router-link class="nav-link" to="/about">About The Team</router-link>
            </li>            
          </ul>
        </div>
      </div>
    </nav>
    <router-view/>
    <Footer/>
  </div>
</template>

<script>

import Footer from './components/Footer';
export default {
  components:{
    Footer
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav{
  padding: 30px;
}

.bg-dark{
  background: #00242c !important;
}
</style>
