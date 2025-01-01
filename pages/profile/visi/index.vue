<template>
  <div class="container-fluid">
    <div class="row p-4">
      <div class="col-md-3 mb-2">
        <div class="card shadow p-5" style="width: 100%">
          <img src="../../../assets/smk.png" alt="SMK Logo" class="img-fluid" />
        </div>
      </div>
      <div class="col-md-9">
        <div class="card shadow p-5" style="width: 100%">
          <div class="content">
            <h4 class="text-primary">Visi:</h4>
            <p class="visi">
              TERWUJUDNYA LULUSAN YANG CERDAS, AKTIF, KOMPETITIF, ADAPTIF, DAN
              PRODUKTIF BERLANDASKAN IMAN DAN TAKWA (CAKAP BERIMTAK)
            </p>

            <br />
            <h4 class="text-primary">Misi:</h4>
            <ul class="list-unstyled">
              <li><h6>1. Menyiapkan Sumber Daya Manusia yang cerdas dan kompeten baik hardskill maupun softskill.</h6></li>
              <li><h6>2. Meningkatkan dan mengembangkan aktifitas serta kreatifitas seluruh warga sekolah dalam berbagai kegiatan positif.</h6></li>
              <li><h6>3. Mewujudkan manajemen pengelolaan yang efektif, efesien, transparan, akuntabel dan layanan prima.</h6></li>
              <li><h6>4. Menumbuhkan dan mengembangkan potensi dan kemampuan Sumber Daya Manusia yang berdaya saing tinggi melalui berbagai kegiatan akademik maupun non akademik.</h6></li>
              <li><h6>5. Menyelenggarakan berbagai program kegiatan dalam upaya meningkatkan Sumber Daya Manusia yang mampu menyesuaikan dengan perkembangan.</h6></li>
              <li><h6>6. Mengembangkan sarana prasarana dan lingkungan sekolah yang menyenangkan sebagai wadah menumbuhkembangkan daya kreasi dan inovasi untuk menghasilkan produk teknologi tepat guna.</h6></li>
              <li><h6>7. Membangun jiwa wirausaha yang handal melalui pembelajaran Teaching Factory (TEFA) dan Kelas Industri.</h6></li>
              <li><h6>8. Menjalin dan mengembangkan kemitraan dengan Industri dan Dunia Kerja (IDUKA) serta lembaga lainnya yang relevan.</h6></li>
            </ul>

            <br />
            <h4 class="text-primary">Tujuan:</h4>
            <ul class="list-unstyled">
              <li><h6>1. Sekolah meraih prestasi pencapaian nilai rata-rata UN dan indeks integritas diatas rata-rata Nasional pada tahun 2026.</h6></li>
              <li><h6>2. Sekolah Menghasilkan Tamatan yang siap bekerja Minimal 50 % Tamatan bekerja pada tahun tamat.</h6></li>
              <li><h6>3. Terciptanya aktivitas dan kreatifitas yang positif oleh seluruh warga sekolah.</h6></li>
              <li><h6>4. Sekolah meraih prestasi akademik dan non akademik minimal di tingkat provinsi Jawa Barat dan Nasional.</h6></li>
              <li><h6>5. Sekolah memiliki tenaga pendidik dan kependidikan yang berkualifikasi minimal S1 dan linier dengan tugasnya, bersertifikat pendidik dan telah mengikuti diklat implementasi kurikulum merdeka pada tahun 2024.</h6></li>
              <li><h6>6. Sekolah mencapai kriteria sekolah berwawasan lingkungan (adiwiyata) pada tahun 2026.</h6></li>
              <li><h6>7. Sekolah terakreditasi dengan Nilai A pada tahun 2024.</h6></li>
              <li><h6>8. Sekolah memiliki Lembaga Sertifikasi Profesi (LSP) yang terlisensi, Tempat Uji Kompetensi (TUK) yang terverifikasi dan Bursa Kerja Khusus (BKK) yang terakreditasi pada tahun 2025.</h6></li>
              <li><h6>9. Sekolah memiliki Perpustakaan yang terakreditasi A pada tahun 2026.</h6></li>
              <li><h6>10. Sekolah menjadi Badan Layanan Umum Daerah (BLUD) pada tahun 2025.</h6></li>
              <li><h6>11. Sekolah mengimplementasikan Kurikulum Merdeka untuk seluruh tingkat pada tahun 2024.</h6></li>
              <li><h6>12. Sekolah memiliki Dokumen Kurikulum Merdeka untuk seluruh tingkat pada tahun 2024</h6></li>
              <li><h6>13. Sekolah menerapkan Kurikulum Merdeka dengan Pembelajaran Berdiferensiasi dan Pembelajaran Sosial-Emosional untuk seluruh tingkat pada tahun 2024.</h6></li>
              <li><h6>14. Sekolah memiliki sarana prasarana sesuai dengan standar pelayanan minimal pendidikan dan standar IDUKA pada tahun 2026.</h6></li>
              <li><h6>15. Sekolah memiliki Teaching Factory di semua program keahlian yang sesuai dengan standar industri dan representatif pada tahun 2024.</h6></li>
              <li><h6>16. Sekolah melaksanakan program menumbuh kembangkan Budi Pekerti dan akhlak mulia melalui pendidikan karakter pada kegiatan, intra, ekstra kurikuler dan non kurikuler.</h6></li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
useHead({ title: "Visi & Misi" })
</script>

<style scoped>
.card {
  border-radius: 10px;
}

.content h4, .content h6 {
  margin-bottom: 15px;
}

ul {
  padding-left: 20px;
}

ul li h6 {
  margin-bottom: 10px;
}
.img-fluid {
  max-width: 100%;
  height: auto;
}
@media (max-width: 768px) {
  .visi{
    text-align: center;
  }
}
</style>
