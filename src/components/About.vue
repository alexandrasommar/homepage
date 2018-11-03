<template>
  <div class="container about">
    <h1>About.</h1>
    <p>I'm a developer. I know:</p>
    <ul>
      <li>HTML</li>
      <li>CSS</li>
      <li>PHP</li>
      <li>JavaScript</li>
      <li>SQL</li>
      <li>C#</li>
    </ul>


  </div>

</template>
<script>
  export default {
    name: 'about',
  };
</script>
<style>
  .about {
    background: linear-gradient(90deg, #69b7ebbf, #b3dbd3c4, #f4d6dbd9),
    url('../assets/mountain.jpg');
    background-size: cover;
    background-position: center;
    display: flex;
    flex-direction: column;
    align-items: center;

  }
</style>
