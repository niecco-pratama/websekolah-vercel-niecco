<!-- <script setup>

import AboutCard from '../components/AboutCard.vue'
import TeamCard from '../components/TeamCard.vue'

const daftarteam = [
{nama: 'John Doe', jabatan: 'CEO'},
{nama: 'Jane Smith', jabatan: 'CTO'},
{nama: 'Mike Johnson', jabatan: 'CFO'},
  ]
</script>

<template>
  <main>
    <div class="kotak">
      <h1>Tentang Kami</h1>
    </div>
    <section class="about-section">
      <div class="about-teks">
            <p>Certita adalah platform yang menyediakan berbagai layanan dan informasi terkait sertifikasi. Kami berkomitmen untuk memberikan pengalaman terbaik bagi pengguna kami.</p>
            <p>Dengan berbagai fitur dan layanan yang kami tawarkan, kami berharap dapat membantu individu dan organisasi dalam mencapai tujuan sertifikasi mereka dengan lebih mudah dan efisien.</p>
      </div>

      <div class="team-section">
        <h2>Tim Kami</h2>
        <div class="container">
          <TeamCard
            v-for="team in daftarteam"
            :key="team.nama"
            :nama="team.nama"
            :jabatan="team.jabatan"
           
          />
        </div>
      </div>
    </section>
  </main>
</template>

<style scoped>
 /* video {
 margin-top: 16px;
  border-radius: 10px;
  display: block;
  } */
.about-section {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: 20px;
}
.about-teks {
  flex: 1;
}

  .container {
  font-family: 'Segoe UI', sans-serif;
  display: flex;
  place-content: center;
  flex-wrap: wrap;
  }

  .container h1 {
   background: linear-gradient(to bottom, #4e7eb4, #3b588d);
   -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    margin-bottom: 10px;
    text-align: center;
    width: 100%;

   }

   .kotak {
   color: white;
   width: 100%;
   height: 100px;
   background: linear-gradient(to bottom, #4e7eb4, #3b588d);
   box-shadow: 0px 1px 2px rgba(0, 0, 0, 0.4);
   overflow: hidden;
   margin: 15px;
   padding: 24px;
   text-align: center;
   }
   </style> -->

   <template>

    <h2 class="hero"><b>Tentang Kami</b></h2>

    <div class="about">
      <div class="cerita">
        <div class="teks">
          <h1><b>CERITA KAMI</b></h1>

          <p><b>
            Toko kami di buat untuk orang yang
            membutuhkan pakian atau aksesoris yang di inginkan.
            </b>
          </p>

          <p><b>
            kami berusaha menyediakan produk yang bagus
            dengann harga yang terjangkau.Kami juga selalu berusaha
            memberikan pelayanan yan ramah kepada pelanggan.
            </b>
          </p>
        </div>
          <div class="gambar">
          <div class="palceholder">
          <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSsoB8Fd1XXYzbEfmH65nWCXE-3Lqpl1N5qmyb1KuwhQw&s=10" alt="Deskripsi" width="400" >
          </div>
        </div>
      </div>
    </div>

    <section class="features-section">
  <div class="features-container">
    
    <!-- Fitur 1 -->
    <div class="feature-card">
      <div class="icon">💀</div>
      <h3><b>AKBAR</b></h3>
      <p><b>MANAGER</b></p>
    </div>

    <!-- Fitur 2 -->
    <div class="feature-card">
      <div class="icon">😎</div>
      <h3><b>NIECCO</b></h3>
      <p><b>CEO MAPAN</b></p>
    </div>

    <!-- Fitur 3 -->
    <div class="feature-card">
      <div class="icon">☠️</div>
      <h3><b>FAIZA</b></h3>
      <p><b>STAFF</b></p>
    </div>

  </div>
</section>

   </template>

   <style scoped>
  .about {
    padding: 50px;
  }

  .cerita {
    display: flex;
    align-items: center;
    gap: 100px;
  }

  .teks{
    font-size: 35px;
    margin-bottom: 30%;
  }
  .gambar {
    
    height: 400px;
  }

  .hero{
    font-size: 40px;
    text-align: center;
    padding: 30px;
    border-radius: 20px;
    background-color: aqua;
    color: rgb(0, 0, 0);
    margin: 40px
    
  }
  p{
    font-size: 20px;
  }
  
  .features-section {
  padding: 50px 20px;
  background-color:   rgb(83, 173, 185)
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
  box-shadow: 0 4px 12px rgb(0, 0, 0); /* Memberikan efek kartu melayang */
  transition: transform 0.2s ease;
}

.feature-card:hover {
  transform: translateY(-5px); /* Efek sedikit naik saat di-hover */
}

  </style>