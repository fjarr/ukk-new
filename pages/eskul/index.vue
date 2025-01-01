<template>
  <div class="container-fluid">
    <div class="judul text-center mt-5">
      <h4 class="text-secondary">EKSTRAKULIKULER</h4>
      <h6 class="text-primary">SMKN 4 TASIKMALAYA</h6>
    </div>
    <div class="content p-5">
      <div class="row text-center">
        <div class="col-6 col-md-3 col-lg-2 mb-4">
          <img src="../../assets/eskul/basket.jpg" alt="Basket" class="eskul-img">
          <h4 class="pt-2">BASKET</h4>
        </div>
        <div class="col-6 col-md-3 col-lg-2 mb-4">
          <img src="../../assets/eskul/bd.jpg" alt="Bulu Tangkis" class="eskul-img">
          <h4 class="pt-2">BULU TANGKIS</h4>
        </div>
        <div class="col-6 col-md-3 col-lg-2 mb-4">
          <img src="../../assets/eskul/cj.jpg" alt="Cinematografi & Jurnalistik" class="eskul-img">
          <h4 class="pt-2">CINEMATOGRAFI & JURNALISTIK</h4>
        </div>
        <div class="col-6 col-md-3 col-lg-2 mb-4">
          <img src="../../assets/eskul/e.jpg" alt="English Club" class="eskul-img">
          <h4 class="pt-2">ENGLISH CLUB</h4>
        </div>
        <div class="col-6 col-md-3 col-lg-2 mb-4">
          <img src="../../assets/eskul/it.jpg" alt="IT Club" class="eskul-img">
          <h4 class="pt-2">IT CLUB</h4>
        </div>
        <div class="col-6 col-md-3 col-lg-2 mb-4">
          <img src="../../assets/eskul/laskar.jpg" alt="Laskar Pustaka" class="eskul-img">
          <h4 class="pt-2">LASKAR PUSTAKA</h4>
        </div>
        <div class="col-6 col-md-3 col-lg-2 mb-4">
          <img src="../../assets/eskul/paskib.jpg" alt="Paskibra" class="eskul-img">
          <h4 class="pt-2">PASKIBRA</h4>
        </div>
        <div class="col-6 col-md-3 col-lg-2 mb-4">
          <img src="../../assets/eskul/pd.jpg" alt="Perisai Diri" class="eskul-img">
          <h4 class="pt-2">PERISAI DIRI</h4>
        </div>
        <div class="col-6 col-md-3 col-lg-2 mb-4">
          <img src="../../assets/eskul/pks.jpg" alt="Polisi Keamanan Sekolah" class="eskul-img">
          <h4 class="pt-2">POLISI KEAMANAN SEKOLAH</h4>
        </div>
        <div class="col-6 col-md-3 col-lg-2 mb-4">
          <img src="../../assets/eskul/plh.jpg" alt="Pendidikan Lingkungan Hidup" class="eskul-img">
          <h4 class="pt-2">PENDIDIKAN LINGKUNGAN HIDUP</h4>
        </div>
        <div class="col-6 col-md-3 col-lg-2 mb-4">
          <img src="../../assets/eskul/pmr.jpg" alt="Palang Merah Remaja" class="eskul-img">
          <h4 class="pt-2">PALANG MERAH REMAJA</h4>
        </div>
        <div class="col-6 col-md-3 col-lg-2 mb-4">
          <img src="../../assets/eskul/pram.jpg" alt="Pramuka" class="eskul-img">
          <h4 class="pt-2">PRAMUKA</h4>
        </div>
        <div class="col-6 col-md-3 col-lg-2 mb-4">
          <img src="../../assets/eskul/futsal.jpeg" alt="Futsal" class="eskul-img">
          <h4 class="pt-2">FUTSAL</h4>
        </div>
        <div class="col-6 col-md-3 col-lg-2 mb-4">
          <img src="../../assets/eskul/voly.jpeg" alt="Voly" class="eskul-img">
          <h4 class="pt-2">VOLY</h4>
        </div>
        <div class="col-6 col-md-3 col-lg-2 mb-4">
          <img src="../../assets/eskul/bola.jpeg" alt="Sepak Bola" class="eskul-img">
          <h4 class="pt-2">SEPAK BOLA</h4>
        </div>
        <div class="col-6 col-md-3 col-lg-2 mb-4">
          <img src="../../assets/eskul/irma.jpeg" alt="IRMA" class="eskul-img">
          <h4 class="pt-2">IRMA</h4>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.eskul-img {
  width: 100%;
  height: 180px;
  object-fit: cover;
  border-radius: 50%;
  transition: transform 0.3s ease;
}

.eskul-img:hover {
  transform: scale(1.1);
}

.pt-2 {
  padding-top: 0.5rem;
}

.text-center h4 {
  font-size: 1.1rem;
  font-weight: bold;
}

@media (max-width: 768px) {
  .col-6 {
    padding-left: 10px;
    padding-right: 10px;
  }
  .eskul-img {
    height:120px;
  }

}
</style>

<script setup>
useHead({ title: "Ekstrakulikuler" })
</script>
