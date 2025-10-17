<template>
  <div >
    <div class="main-content-wrapper"> <h1>Графіті</h1>
    </div>
    <p class="p">Культура графіті — це вуличне мистецтво, що виникло в кінці 1960-х років у Нью-Йорку як спосіб самовираження, що розвинувся від простих написання псевдонімів ("тегів") до складних, стилізованих зображень. 
      </p>
      <div><h3>Графіті не пішло від Фрески!</h3>
      <img alt="fresca" src="https://decorcdn.com/img/catalog-240/freska-2025.jpg">
      <img alt="graffiti" src="https://tvoemisto.tv/media/gallery/full/c/o/collage2_e8754.jpg">
      </div>
      <p> Фрески: Це стародавня техніка живопису на стінах, яка існувала тисячі років.</p>

      <p> 
Графіті: Термін "графіті" походить від італійського "graffiti", що означає "надряпані". Це стосується найдавніших написів, зроблених гострими предметами. Сучасне вуличне графіті, як субкультура, з'явилося у 20-му столітті. </p>
  </div>

</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<style scoped>

img {
  height: 200px;

}

p{

  font-size: 25px;
  
  color:rgb(255, 255, 255); /* основний колір */
  text-transform: uppercase;
  text-shadow:
    -2px -2px 0 #000,
     2px -2px 0 #000,
    -2px  2px 0 #000,
     2px  2px 0 #000,
     0  0 10px #f71909,
     0  0 20px #ff9100;

}


.p{
  font-family: 'Comic Sans MS', 'Impact', cursive; /* або підключи свій шрифт */
  font-size: 30px;
  font-weight: 900px;
  color: #03ffc0; /* основний колір */
  text-transform: uppercase;
  text-shadow:
    -2px -2px 0 #000,
     2px -2px 0 #000,
    -2px  2px 0 #000,
     2px  2px 0 #000,
     0  0 10px #f71909,
     0  0 20px #ff9100;
  letter-spacing: 3px;
  transition: transform 0.3s ease, text-shadow 0.3s ease;
}
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}



</style>
