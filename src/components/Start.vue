<template>
  <div class="start-container">
    <div class="container start">
      <h1>Hello.</h1>
      <p>My name is Alexandra Sommar and I'm a developer based in Gothenburg, Sweden.</p>
      <p>Here you'll find a few of my projects and contact info.</p>
      <div class="icons">
        <a href="mailto:alexandra@sommar.se">
          <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-mail"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"/><polyline points="22,6 12,13 2,6"/></svg>
        </a>
        <a href="https://github.com/alexandrasommar" target="_blank" rel="noopener noreferrer">
          <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-github"><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"/></svg>
        </a>
        <a href="https://www.linkedin.com/in/alexandra-sommar" target="_blank" rel="noopener noreferrer">
          <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-linkedin"><path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"/><rect x="2" y="9" width="4" height="12"/><circle cx="4" cy="4" r="2"/></svg>
        </a>
      </div>
      <div class="gradient" />
    </div>
    <div class="coachella">
      <figcaption>
        <h3>#coachellamoment</h3>
      </figcaption>
    </div>
    <div class="blog">
      <a href="http://alexandrasommar.se/blogg">
        <figcaption>
          <h3>blog</h3>
        </figcaption>
      </a>
    </div>
  <about/>
  <div class="bulldada">
    <a href="http://alexandrasommar.se/cultofbulldada">
      <figcaption>
        <h3>bulldada</h3>
      </figcaption>
    </a>
  </div>
  <div class="animation">
    <a href="http://alexandrasommar.se/animation">
      <figcaption>
        <h3>animation</h3>
      </figcaption>
    </a>
  </div>
</div>
</template>

<script>
  import About from '@/components/About';

  export default {
    name: 'start',
    components: {
      about: About,
    },
  };
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
  .container {
      margin: 0;
      width: 100%;
  }
  .start {
    background: #fff;
    color: #000;
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .start h1 {
    color: #000;
    border-bottom: 5px solid #000;
    clip-path: polygon(25% 0%, 100% 0%, 75% 100%, 0% 100%);
    padding: 0 25px;
  }
  .start p {
    color: #000;
  }
  .icons {
    display:flex;
    justify-content: space-between;
    //align-self:center;
    background-color: #fff;
    position:relative;
    overflow:hidden;
    width: 87%;
  }
  svg {
    width: 70px;
    height: 70px;
    fill:none;
    stroke-width:1px;
    stroke: #000;
    mix-blend-mode:multiply;
    color:#000;
    position:relative;
    opacity:.9;
    display:block;
  }
  svg:hover{
    cursor:pointer;
    transform: scale(.9);
  }
  .gradient {
    position: absolute;
    width: 100%;
    height: 64%;
    //top: -25%;
    //left: -25%;
    mix-blend-mode: screen;
    pointer-events: none;
    background: linear-gradient(55deg, #cb60b3 0%,#9c18dd 44%,#48a7e2 100%);
  }
  h1 {
    color: #fafafa;
    border-bottom: 5px solid #fafafa;
    clip-path: polygon(25% 0%, 100% 0%, 75% 100%, 0% 100%);
    padding: 0 25px;
  }
  p, ul{
    color: #fff0f0;
    width: 85%;
  }
  @keyframes borderAnimation {
      0% {
        border-top: 10px solid #2c3e50;
      }

      20% {
        border-top: 8px;
      }
      80% {

        border-top: 2px;
      }
      100% {
        border-top: 0px;
      }
    }
  .coachella {
    background:
    url('../assets/coachella.png');
    background-size: cover;
    background-position: center;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 300px;
  }
  figcaption {
    color: #fff;
    clip-path: polygon(25% 0%, 100% 0%, 75% 100%, 0% 100%);
    background: #00000096;
    padding: 0 70px;
    font-weight: normal;
  }
  .coachella:hover, .blog:hover, .bulldada:hover, .animation:hover {
    cursor: pointer;
    filter: brightness(110%);
  }


  .blog {
    background:
    url('../assets/volvo.jpg');
    background-size: cover;
    background-position: center;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 300px;
  }

  .bulldada {
    background:
    url('../assets/cultofbulldada.png');
    background-size: cover;
    background-position: center;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 300px;
  }
  .animation {
    background:
    url('../assets/bubbles.png');
    background-size: cover;
    background-position: center;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 300px;
  }
  @media (min-width: 449px) {
    .gradient {
      height: 60%;
    }
  }
  @media (min-width: 700px) {
    .icons {
      //margin-top: 5%;
    }
    .gradient {
      height: 55%;
    }
  }
  @media (min-width: 890px) {
    .start-container {
      display: grid;
      grid-template-columns: 1fr 1fr;
      grid-template-rows: 1fr 1fr 1fr;

      width: 100%;
    }
    .coachella, .blog, .bulldada, .animation {
      height: 500px;
    }
    .icons {
      margin-top: 15%;
    }
    .gradient {
      width: 50%;
      height: 500px;
    }
  }

</style>
