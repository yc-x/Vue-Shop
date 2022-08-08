<template>
  <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
  </nav>
  <div class="container">

  </div>
  <router-view/>
</template>

<style lang="scss">
@import 'node_modules/bootstrap/scss/bootstrap';

  .dropdown-clip {
    overflow: hidden;
  }

  .dropdown-enter-active,
  .dropdown-leave-active {
    transition: all .5s ease-in-out;
    transform: auto;
  }

  .dropdown-enter-from, 
  .dropdown-leave-to {
    opacity: 0;
    transform:translateY(-300px);
  }

  .products-enter-active,
  .products-leave-active {
    transition: all .5s ease-in-out;
  }

  .products-enter-from {
    opacity: 0;
    transform:translateX(300px);
  }
  
  .products-leave-to {
    opacity: 0;
    transform:translateX(-300px);
  }
</style>
