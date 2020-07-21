<template>
  <div id="app">
    
    <router-view/>
  </div>
</template>

<style lang="scss">
/* width */
::-webkit-scrollbar {
  width: 8px;
}

/* Track */
::-webkit-scrollbar-track {
  background: #f1f1f1;
}

/* Handle */
::-webkit-scrollbar-thumb {
  background: rgb(189,139,40);;
}

/* Handle on hover */
::-webkit-scrollbar-thumb:hover {
  background: #555;
}


$brown: rgb(189,139,40);

#app {
  font-family: Dosis, Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

.nav-item {
  //padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: $brown;
    }
  }
}

.body {
    margin-top: 7rem;
}

.button {
  border-image-repeat: stretch;
  border-radius: 4.8px;
  padding: 0 8px;
  vertical-align: middle;
}

.button-brown {
  background: $brown;
  border: 1px solid $brown;
  color: $brown;
}


</style>
