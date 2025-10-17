<template>
  <div class="app-container">
    <!-- Основний контент -->
    <main class="content">
      <h1 class="title">Графіті</h1>
      <p class="text">
        Культура графіті — це вуличне мистецтво, що виникло в кінці 1960-х років у Нью-Йорку як спосіб самовираження, що розвинувся від простих написання псевдонімів ("тегів") до складних, стилізованих зображень.
      </p>

      <section class="comparison">
        <h3>Графіті не пішло від фрески</h3>
        <div class="images">
          <img src="https://decorcdn.com/img/catalog-240/freska-2025.jpg" alt="Фреска" class="comparison-image">
          <img src="https://tvoemisto.tv/media/gallery/full/c/o/collage2_e8754.jpg" alt="Графіті" class="comparison-image">
        </div>
        <p>Фрески — стародавня техніка живопису на стінах, яка існувала тисячі років.</p>
        <p>Графіті: Термін "графіті" походить від італійського "graffiti", що означає "надряпані". Це стосується найдавніших написів, зроблених гострими предметами. Сучасне вуличне графіті з'явилося у 20-му столітті.</p>
      </section>
    </main>

    <!-- Футер -->
    <footer class="footer">
      <div class="footer-sections">
        <section class="footer-section">
          <h3 class="footer-title">🎨 Залишай свій слід</h3>
          <p>Маєш стінопис або ідею для нашого сайту?</p>
          <p>
            Надсилай творчість на: 
            <a href="mailto:submit@grafiti-project.com" class="footer-link">submit@grafiti-project.com</a>
          </p>
        </section>

        <section class="footer-section">
          <h3 class="footer-title">🔗 Поділись посиланням</h3>
          <p>Встав URL свого графіті (Imgur, Instagram тощо):</p>
          <form @submit.prevent="submitUrl" class="url-form">
            <input type="url" v-model="imageUrl" placeholder="Вставте URL..." required class="url-input">
            <button type="submit" class="url-submit">Надіслати</button>
          </form>
          <p v-if="submissionMessage" class="submission-message">{{ submissionMessage }}</p>
        </section>
      </div>
      <div class="footer-bottom">
        &copy; {{ currentYear }} Graffiti Project трохи використовував нейросеть бо я тупий
      </div>
    </footer>
  </div>
</template>

<style scoped>

.app-container {
  font-family: Arial, sans-serif;
  color: #222;
  background-color:rgba(249, 249, 249, 0.41);
  line-height: 1.5;
  max-width: 900px;
  margin: 0 auto;
  padding: 20px;
}

.title {
  font-size: 32px;
  margin-bottom: 15px;
}
.text {
  font-size: 16px;
  margin-bottom: 15px;
}

.comparison {
  margin-top: 20px;
}

.images {
  display: flex;
  gap: 15px;
  margin: 10px 0;
}

.comparison-image {
  width: 100%;
  max-width: 400px;
  border-radius: 4px;
  border: 1px solid #ccc;
}


.footer-sections {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  justify-content: space-between;
  
}

.footer-section {
  flex: 1;
  min-width: 200px;
  
}

.footer-title {
  font-weight: bold;
  margin-bottom: 8px;
  font-size: 16px;
  
}

.footer-link {
  color:rgb(255, 0, 0);
  text-decoration: none;
  
}

.url-form {
  margin-top: 5px;
}

.url-input {
  width: 100%;
  padding: 8px;
  margin-bottom: 8px;
  border-radius: 4px;
  border: 1px solid #ccc;
}

.url-submit {
  padding: 8px 12px;
  border: none;
  border-radius: 4px;
  background-color:#a35c22;
  color: #222;
  cursor: pointer;
  
}

.url-submit:hover {
  background-color:rgb(190, 169, 83);
  
}

.footer-bottom {
  text-align: center;
  margin-top: 15px;
  font-size: 14px;
}
</style>
