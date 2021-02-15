<template>
  <div>
    <router-link to="/">Home</router-link>|
    <router-link to="/about">About</router-link>

    <div id="logo">
      <img class="uk-width-1-1" src="./assets/logo.png" />
    </div>

    <router-link to="/test-bug">
      <!-- vvv UNCOMMENT THESE LINE AND RUN `npm run build` SO THE ERROR SHOW UP -->
      <!-- <div id="logo">
        <img class="uk-width-1-1" src="./assets/logo.png" />
      </div> -->
    </router-link>

    <router-view v-slot="{ Component }">
      <Suspense>
        <component :is="Component" />
      </Suspense>
    </router-view>
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
