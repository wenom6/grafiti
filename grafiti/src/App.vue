<template>
  <img alt="Vue logo" src="./assets/grafiti.jpg">
  <FooterComponent/>
  <HelloWorld/>
  
</template>

<script>

import HelloWorld from './components/HelloWorld.vue'
import FooterComponent from './components/FooterComponent.vue'

export default {
  name: 'app',
  components: {
    HelloWorld,
        FooterComponent,
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
  background-size: 120%; /* 👉 міняй це значення, щоб змінювати розмір фону */
  filter: blur(8px); /* 👉 тут міняй ступінь розмиття */
  z-index: -1;
}


</style>
