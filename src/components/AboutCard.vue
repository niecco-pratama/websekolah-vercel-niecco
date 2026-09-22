<template>
    <div class="kolom">
      
      
    </div>
</template>
 
<style scoped>
.kolom {
      font-family: 'segoe UI', sans-serif;
    display: flex;

    margin: 50px;
    flex: 1;
    flex-direction: row;
    overflow: hidden;
    background-color: lightskyblue; /* Warna latar belakang */
}

.gambar img{
    width: 4%;
    height: auto;
    border-radius: 10px; /* Membuat sudut gambar melengkung */
}
.teks {
    flex: 1;
}
.teks h1{
    background-color: linear-gradient(to bottom, #4facfe, #00f2fe); /* Gradient biru */
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    margin-bottom: 10px;
}

.teks p {
    margin-top: 0;
}
</style>