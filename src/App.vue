<template>
  <div id="app">
    <app-header></app-header>
    <main>
      <router-view/>
    </main>
    <app-footer></app-footer>
  </div>
</template>

<script>
import Header from '@/components/Header';
import Footer from '@/components/Footer';

export default {
  name: 'App',
  components: {
    'app-header': Header,
    'app-footer': Footer,
  },
};
</script>

<style>
html, body, h1, h2, h3, p{
  margin: 0;
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
