<template>
  <img alt="Vue logo" src="./assets/grafiti.jpg">

  <HelloWorld/>
  
</template>

<script>

import HelloWorld from './components/HelloWorld.vue'


export default {
  name: 'app',
  components: {
    HelloWorld,

  }
}
</script>

<style >


#app {
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
#app::before {
  content: "";
  position: absolute;
  inset: 0;
  background-image: url('https://png.pngtree.com/thumb_back/fh260/background/20250914/pngtree-abstract-painted-wall-colorful-graffiti-patterns-urban-street-art-style-image_19358183.webp');
  background-size: 120%; 
  filter: blur(8px); 
  z-index: -1;
}


</style>
