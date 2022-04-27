<template>
  <div id="app">
    <div class="nav">
      <router-link class="logo" to="/">Reddit</router-link>

      <div class="links">
        <router-link to="/favorites">Favorites</router-link>
      </div>
    </div>
    <router-view />
  </div>
</template>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: sans-serif;
  width: 100vw;
  height: 100vh;
  color: #2c3e50;
  overflow-x: hidden;
}

#app {
  width: 100%;
  height: 100%;
  width: 80%;
  margin: auto;
}

.nav {
  display: flex;
  padding: 20px 0px;
  justify-content: space-between;
  align-items: center;
}

.links {
  // display: flex;
  // justify-content: space-between;
  // flex: 1;

  a {
    font-weight: bold;
    text-transform: uppercase;
    text-decoration: none;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}

.logo {
  color: #42b983;
  flex: 5;
  font-weight: bold;
  text-decoration: none;
  font-size: 2rem;
}

@media screen and (max-width: 950px) {
  .logo {
    flex: 4;
  }
}

@media screen and (max-width: 700px) {
  .logo {
    flex: 3;
  }
}

@media screen and (max-width: 550px) {
  .logo {
    flex: 2;
  }
}

@media screen and (max-width: 400px) {
  .logo {
    flex: 1.5;
  }
}
</style>
