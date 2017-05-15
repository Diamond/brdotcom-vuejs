<template>
  <div id="app">
    <nav-bar />
    <about />
    <posts />
    <div class="divider" />
    <projects />
    <div class="divider" />
    <presentations />
    <custom-footer />
  </div>
</template>

<script>
import NavBar from './components/NavBar';
import About from './components/About';
import Posts from './components/Posts';
import Projects from './components/Projects';
import Presentations from './components/Presentations';
import CustomFooter from './components/CustomFooter';

export default {
  name: 'app',
  components: {
    NavBar,
    About,
    Posts,
    Projects,
    Presentations,
    CustomFooter
  }
};
</script>

<style>

</style>
