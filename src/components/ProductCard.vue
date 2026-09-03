<script setup>
import { ref } from 'vue'

defineProps(['nama', 'harga', 'gambar'])

const gambarDipilih = ref(null)

function bukaPreview(src) {
  gambarDipilih.value = src // isi: src gambar yang diklik
}
function tutupPreview() {
  gambarDipilih.value = null
}
// fitur suara
function tambahKeKeranjang(nama) {
  // Logika untuk menambahkan produk ke keranjang
  const suara = new Audio('nikin-pop-up-something-160353.mp3') // Ganti dengan path suara yang sesuai
  suara.play()
  alert(`${nama} telah ditambahkan ke keranjang!`)
}
</script>
<template>
  <div class="card">
    <img :src="gambar" :alt="nama" @click="bukaPreview(gambar)" />
    <h3>{{ nama }}</h3>
    <p>Rp {{ harga.toLocaleString('id-ID') }}</p>
    <button class="btn-grad" @click="tambahKeKeranjang">Tambah ke Keranjang</button>
  </div>

  <div v-if="gambarDipilih" class="preview-overlay">
    <img :src="gambarDipilih" class="preview-besar" />
    <button @click="tutupPreview" class="btn-grad">Tutup</button>
  </div>
</template>

<style scoped>
.card {
  border: 1px solid #ddd;
  border-radius: 10px;
  padding: 14px;
  width: 200px;
  text-align: center;
}
.card img {
  width: 100%;
  border-radius: 6px;
}
.btn-grad {
  background-image: linear-gradient(to right, #112cc9 0%, #0462f0 51%, #1ec4f7 100%);
}

.btn-grad {
  margin: 10px;
  padding: 10px 35px;
  text-align: center;
  text-transform: uppercase;
  transition: 0.5s;
  background-size: 200% auto;
  color: white;
  box-shadow: 0 0 20px #eee;
  border-radius: 10px;
  display: block;
  outline: none;
  border: none;
}

.btn-grad:hover {
  background-position: right center;
  color: #fff;
  text-decoration: none;
}

.preview-overlay {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.7);
  display: flex;
  align-items: center;
  justify-content: center;
}
.preview-besar {
  max-width: 80%;
  max-height: 80%;
  border-radius: 8px;
}
</style>