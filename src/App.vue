<template>
  <div id="app">
    <nav>
      <a href="http://alexandrasommar.se">
        <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-moon"><path d="M21 12.79A9 9 0 1 1 11.21 3 7 7 0 0 0 21 12.79z"/></svg>
      </a>
    </nav>

    <router-view/>

  </div>
</template>

<script>
import About from '@/components/About';

export default {
  name: 'app',
  components: {
    about: About,
  },
};
</script>

<style>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;

    color: #2c3e50;
    margin: 0;
    //display: grid;

    overflow-x: hidden;



  }
  nav {
    transition: all 2s;
   position: absolute;
   top: 10px;
   left: 9px;
   z-index: 1500;
  }
  nav svg {
    height: 50px;
    width: 50px;
    transition: transform .8s ease-in-out;
  }
  nav svg:hover {
    scale: 1;
    transform: rotate(240deg);
  }
  input {
    display: none;
  }
  input~ul {

    background: #fffc;
    width: 100vw;
    height: 100vh;
    list-style: none;
    transition: all 0s;
position: fixed;
left: -9000px;
  }

  input:checked~ul {


    width: 100vw;
    height: 100vh;
    //z-index: 1500;
    transition: all 0s;
      position: relative;
      left: 0;

    display: flex;
    flex-direction: column;
    //justify-content: center;
    align-items: center;
  }
  nav a {
    color: #000;
    text-decoration: none;
    text-transform: uppercase;
  }
  nav li {
    width: 100%;
    padding: 3%;
    text-align: center;
  }
  img {
    max-width: 100%;
  }
  img:hover {
    cursor: pointer;
   filter: brightness(110%);
  }
  body {
    background: #fcfcfc;
    margin: 0;

  }


</style>
