<script setup>

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
   </style>