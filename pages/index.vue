<template>
  <div class="hero-section">
    <div class="overlay"></div>
    <div class="content">
      <h1>Selamat Datang di <span class="highlight">SMKN 4 Tasikmalaya</span></h1>
      <p>A Place Full Of</p>
      <hr />
      <p class="description">
        WHERE AN EMPTY MIND BECOME AN OPEN MIND<br />
        WHERE STRANGERS BECOME BEST FRIENDS
      </p>
    </div>
  </div>

  <footer class="footer">
    <div class="footer-column">
      <h3>SMKN4TASIKMALAYA.COM</h3>
      <p>
        Dikembangkan untuk mempromosikan <i>civitas akademika</i> dan 
        <i>stakeholder</i> di SMKN 4 Tasikmalaya. Dikelola secara terbuka, 
        partisipatif, dan memberikan kesempatan pada siswa SMKN 4 Tasikmalaya
        untuk mengasah keterampilan jurnalistik, kehumasan, dan pengembangan 
        website.
      </p>
    </div>
    <div class="footer-column">
      <h3>CORE VALUES</h3>
      <p>
        Kami percaya bahwa dengan pengetahuan, bimbingan yang tepat, dan 
        kebijaksanaan dari seniornya maka generasi muda mampu melejit 
        dan menorehkan pencapaian melebihi ekspektasi.
      </p>
    </div>
    <div class="footer-column">
      <h3>JOIN US!</h3>
      <p>
        Kami menyambut dengan tangan terbuka siswa SMKN 4 Tasikmalaya dan 
        tertarik di dunia jurnalistik dan pengembangan website.<br /><br />
        Jangan sungkan, hilangkan keraguan. Karena kamu bisa belajar dari 
        awal dengan bimbingan para senior.
      </p>
    </div>
    <div class="footer-column">
      <h3>MARI BERKOLABORASI</h3>
      <p>
        Akang / Teteth memiliki ide kolaborasi? Kami sangat ingin 
        mendengarnya, kapan kita bisa diskusi?<br /><br />
        <a href="#" class="contact-link">Kontak Kami!</a>
      </p>
    </div>
  </footer>
</template>

<script>
export default {
  name: "HeroSection",
};
</script>

<style scoped>
.hero-section {
  position: relative;
  height: 100vh;
  background-image: url('../asset/img/images.jpg'); /* Ganti dengan URL gambar Anda */
  background-size: cover;
  background-position: center;
  display: flex;
  align-items: center;
  justify-content: center;
  color: white;
  font-family: Arial, sans-serif;
  text-align: center;
}

.overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.5);
}

.content {
  position: relative;
  z-index: 2;
}

h1 {
  font-size: 3rem;
  margin: 0;
}

.highlight {
  font-weight: bold;
}

p {
  font-size: 1.5rem;
  margin: 10px 0;
}

hr {
  width: 100px;
  height: 2px;
  background-color: white;
  border: none;
  margin: 20px auto;
}

.description {
  font-size: 1rem;
  line-height: 1.5;
}

.footer {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 20px;
  background-color: #111;
  color: #fff;
  padding: 40px;
  font-family: Arial, sans-serif;
}

.footer-column {
  line-height: 1.8;
}

.footer-column h3 {
  font-size: 1.2rem;
  margin-bottom: 10px;
  color: #ccc;
  text-transform: uppercase;
}

.footer-column p {
  font-size: 0.9rem;
  color: #aaa;
}

.contact-link {
  color: #fff;
  text-decoration: none;
  font-weight: bold;
}

.contact-link:hover {
  text-decoration: underline;
}
</style>
