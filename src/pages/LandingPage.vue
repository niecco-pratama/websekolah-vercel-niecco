<!-- <template>
  <main>
    <h1>Selamat Datang di Onlineshop Sekolah</h1>
    <p>Belanja gampang, sekolah senang.</p>
  </main>
</template>
 -->

 <template>
  <div class="landing-page">
    <!-- Navbar Header -->
    <header class="navbar">
      <div class="logo">SMK Yadika Soreang — Onlineshop</div>
       </header>

    <!-- Hero Section -->
    <section class="hero-section">
      <h1>Belanja Perlengkapan Sekolah Gaulz.</h1>
      <p>Dari seragam, sampai tas sekolah — semua ada.</p>
      <button class="btn-primary"><RouterLink to="/product">Lihat Produk</RouterLink></button>
    </section>
    <center><video controls width="480" muted loop> 
      <source src="https://www.w3schools.com/html/mov_bbb.mp4" type="video/mp4" /> 
      Browser kamu tidak mendukung pemutaran video. 
    </video> </center>
    
    <section class="features-section">
  <div class="features-container">
    
    <!-- Fitur 1 -->
    <div class="feature-card">
      <div class="icon">👍🤙</div>
      <h3>Kualitas Terjamin Kalcer</h3>
      <p>Bahan dipilih langsung oleh tim sekolah.</p>
    </div>

    <!-- Fitur 2 -->
    <div class="feature-card">
      <div class="icon">🤑👌</div>
      <h3>Harga Bersahabat</h3>
      <p>Harga ramah di kantong siswa.</p>
    </div>

    <!-- Fitur 3 -->
    <div class="feature-card">
      <div class="icon">🏫</div>
      <h3>Ambil di Sekolah</h3>
      <p>Tidak perlu ongkir, ambil di Koperasi.</p>
    </div>

  </div>
</section>
    
  </div>
</template>


<style scoped>
/* Reset & Base Style */
.landing-page {
  font-family: Arial, sans-serif;
  color: #0c0c0c;
}

/* Navbar */
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px 20px;
}

.logo {
  font-weight: bold;
}

.nav-links a {
  margin-left: 15px;
  text-decoration: none;
  color: #000;
  font-size: 14px;
}

/* Hero Section (Banner Biru) */
.hero-section {
  background-color: #0787d1fa; /* Warna latar biru */
  color: rgb(14, 13, 13);
  text-align: center;
  padding: 10px 20px;
  margin:  40px;
  border-radius: 20px; /* biar melengkung */
}

.hero-section h1 {
  font-size: 28px;
  margin-bottom: 10px;
}

.hero-section p {
  font-size: 14px;
  opacity: 0.9;
  margin-bottom: 25px;
}


.btn-primary {
  background-color: #e2e8f0;
  color: #000000;
  border: none;
  padding: 10px 24px;
  font-weight: bold;
  border-radius: 50px;
  cursor: pointer;
}

.features-section {
  padding: 50px 20px;
  background-color:  rgb(41, 99, 107)
}

.features-container {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 30px;
  flex-wrap: wrap; 
  max-width: 1000px;
  margin: 0 auto;
}

.feature-card {
  flex: 1;
  min-width: 250px;
  max-width: 300px;
  padding: 25px 20px;
  background-color: #0993d3;
  border-radius: 10px;
  text-align: center;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.08); /* Memberikan efek kartu melayang */
  transition: transform 0.2s ease;
}

.feature-card:hover {
  transform: translateY(-5px); /* Efek sedikit naik saat di-hover */
}

.icon {
  font-size: 32px;
  margin-bottom: 15px;
}

.feature-card h3 {
  font-size: 1.1rem;
  font-weight: 700;
  color: #111827;
  margin-bottom: 8px;
}

.feature-card p {
  font-size: 0.9rem;
  color: #f8f9fa;
  line-height: 1.4;
  margin: 0;
}

</style>