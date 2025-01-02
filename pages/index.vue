<template>
  <div id="carouselExample" class="carousel slide" data-bs-ride="carousel">
    <div class="carousel-inner">
      <div class="carousel-item active">
        <img src="../assets/1.png" alt="" style="width: 100%" />
      </div>
      <div class="carousel-item">
        <img src="../assets/4.jpg" alt="" style="width: 100%" />
      </div>
      <div class="carousel-item">
        <img src="../assets/3.jpg" alt="" style="width: 100%" />
      </div>
    </div>
    <button class="carousel-control-prev" type="button" data-bs-target="#carouselExample" data-bs-slide="prev">
      <span class="carousel-control-prev-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Previous</span>
    </button>
    <button class="carousel-control-next" type="button" data-bs-target="#carouselExample" data-bs-slide="next">
      <span class="carousel-control-next-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Next</span>
    </button>
  </div>

  <div class="container-fluid">
    <div class="berita">
      <h4 class="text-primary d-flex justify-content-center mt-5">BERITA</h4>
      <h6 class="text-secondary d-flex justify-content-center mb-3">
        SMKN 4 TASIKMALAYA
      </h6>
      <div class="content d-flex justify-content-center">
        <div class="row p-5 berita-scroll">
          <div v-for="(foto, i) in berita" :key="i" class="col-6 col-md-3 p-3">
            <nuxt-link :to="`/${foto.id}`">
              <div class="card" style="height: 100%;">
                <img :src="foto.foto" class="img-fluid " alt=""  />
                <hr>
                <p class="judul-berita p-2">{{ foto.judul }}</p>
              </div>
            </nuxt-link>
          </div>
        </div>
      </div>
    </div>
    <div class="sambutan p-3 d-flex justify-content-center">
      <div class="card p-5 rounded-5 shadow" style="width: 90%;">
        <div class="row  p-2">
          <div class=" col-lg-5 ">
            <img src="../assets/kepala.png" alt="" class="img-fluid rounded-5" />
          </div>
          <div class="col-lg-7">
            <div class="judul-sambutan mb-2">
              <h4 class="text-primary">SAMBUTAN</h4>
              <h6 class="text-secondary">KEPALA SMKN 4 TASIKAMALAYA</h6>
            </div>
            <div class="content-s">
              <p class="fw-bold">Assalamu'alaikum Warahmatullahi Wabarakatuh.</p>
              <p>
                Selamat datang di SMKN 4 Tasikmalaya. Segala puji dan syukur kita panjatkan kehadirat Allah SWT, semoga
                kita semua selalu dalam lindungan-Nya. Atas perkenan-Nya, kami dapat menghadirkan website SMK Negeri 4
                Tasikmalaya ini. Kami berharap dengan adanya website ini, para pengunjung dapat lebih mengenal sekolah
                kami, sehingga dapat mempererat tali silaturahmi antara sekolah dan masyarakat demi kemajuan kita
                bersama.
                Tiada gading yang tak retak, website ini masih dalam proses pengembangan dan masih banyak kekurangan
                yang perlu kami perbaiki. Kritik dan saran yang membangun sangat kami harapkan untuk pengembangan lebih
                lanjut.
                Akhirnya, kami mengucapkan terima kasih yang sebesar-besarnya kepada semua pihak yang tidak dapat
                disebutkan satu per satu, atas bantuan dan fasilitas yang telah diberikan. Semoga semua yang kita
                lakukan bermanfaat bagi masyarakat.
              </p>
              <p class="fw-bold">Wassalamu'alaikum Warahmatullahi Wabarakatuh.</p>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="data-sw rounded-4 p-5 my-2">
      <div class="judul text-center">
        <h4 class="text-primary">DATA PENDIDIK PESERTA DIDIK DAN TENAGA KEPENDIDIKAN</h4>
        <h6 class="text-secondary mb-5">
          SMKN 4 TASIKMALAYA
        </h6>
      </div>
      <div class="content-d p-5">
        <div class="row">
          <div class="col-lg-6 mb-4">
            <div class="card shadow rounded-5 p-3">
              <div class="row px-2 py-2">
                <div class="col-6 text-center">
                  <h6>82</h6>
                </div>
                <div class="col-6 text-center">
                  <h6>GURU</h6>
                </div>
              </div>
            </div>
          </div>
          <div class="col-lg-6 mb-4">
            <div class="card shadow rounded-5 p-3">
              <div class="row px-2 py-2">
                <div class="col-6 text-center">
                  <h6>1400</h6>
                </div>
                <div class="col-6 text-center">
                  <h6>SISWA</h6>
                </div>
              </div>
            </div>
          </div>
          <div class="col-lg-6 mb-4">
            <div class="card shadow rounded-5 p-3">
              <div class="row px-2 py-2">
                <div class="col-6 text-center">
                  <h6>19</h6>
                </div>
                <div class="col-6 text-center">
                  <h6>STAF TU</h6>
                </div>
              </div>
            </div>
          </div>
          <div class="col-lg-6 mb-4">
            <div class="card shadow rounded-5 p-3">
              <div class="row px-2 py-2">
                <div class="col-6 text-center">
                  <h6>8</h6>
                </div>
                <div class="col-6 text-center">
                  <h6>LAINNYA</h6>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="vidio pb-5 m-5">
  <h5 class="text-primary text-center">VIDIO YOUTUBE</h5>
  <h6 class="text-secondary text-center pb-3 mb-3">SMKN 4 TASIKMALAYA</h6>
  <div class="video-wrapper">
    <iframe class="rounded-5" 
      src="https://www.youtube.com/embed/5l2u9rHS36k?si=eTP0ycO7TOGcanOH&autoplay=1" 
      title="YouTube video player" frameborder="0" 
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
      referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
  </div>
  
  <div class="row text-center d-flex justify-content-center pt-3">
    <div class="col-4">
      <p>BULAN BAHASA DAN SASTRA SMK 4</p><hr>
        <iframe class="rounded-5"  width="100%"
          src="https://www.youtube.com/embed/E6tbR0ly5jA?si=YyiYKbQ6cN_L_Be6" 
          title="YouTube video player" frameborder="0" 
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" 
          referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
    </div>
    <div class="col-4">
      
        <iframe class="rounded-5"  width="100%"
          src="https://www.youtube.com/embed/_BUlBVhb4Bk?si=Q1XnjdS0FH8D7_Re" 
          title="YouTube video player" frameborder="0" 
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" 
          referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe><hr>
          <p>VIDIO MODERASI BERAGAMA/TOLERANSI</p>
    </div>
    <div class="col-4">
      <p>VIDIO PROGRAM SMK PK 2024</p><hr>
        <iframe class="rounded-5"  width="100%"
          src="https://www.youtube.com/embed/iBtaSZEneMQ?si=_VK_RgG-WgfWDpxv" 
          title="YouTube video player" frameborder="0" 
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" 
          referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
    </div>
  </div>
</div>

  <div class="judul mt-5">
    <h4 class="text-center text-primary ">PROGRAM KEAHLIAN</h4>
    <h6 class="text-secondary text-center ">
      SMKN 4 TASIKMALAYA
    </h6>
  </div>
  <div class="jurusan pt-5 ">
    <img src="../assets/jurusan.png" style="width: 100%;" alt="">
    <div class="detil py-5 d-flex justify-content-center">
      <nuxt-link to="/jurusan">
        <button type="button" class="btn mx-5 text-light" style="width:60vw; background-color: rgb(52, 88, 197);">INFO
          DETAIL</button>
      </nuxt-link>
    </div>
  </div>
  <div class="patner mt-3">
    <div class="judul-patner">
      <h4 class="text-center text-primary">MITRA INDUSTRI</h4>
      <h6 class="text-secondary text-center">
        SMKN 4 TASIKMALAYA
      </h6>
    </div>
    <div class="scroll-container mt-3">
      <div class="scroll-content">
        <div class="img p-5"><img src="../assets/perusahaan/agate.png" alt=""></div>
        <div class="img p-5"><img src="../assets/perusahaan/ahm.png" alt=""></div>
        <div class="img p-5"><img src="../assets/perusahaan/inovindo.png" alt=""></div>
        <div class="img p-5"><img src="../assets/perusahaan/semesta.png" alt=""></div>
        <div class="img p-5"><img src="../assets/perusahaan/skyline.png" alt=""></div>
        <div class="img p-5"><img src="../assets/perusahaan/cikara.png" alt=""></div>
        <div class="img p-5"><img src="../assets/perusahaan/agate.png" alt=""></div>
        <div class="img p-5"><img src="../assets/perusahaan/ahm.png" alt=""></div>
        <div class="img p-5"><img src="../assets/perusahaan/inovindo.png" alt=""></div>
        <div class="img p-5"><img src="../assets/perusahaan/semesta.png" alt=""></div>
        <div class="img p-5"><img src="../assets/perusahaan/skyline.png" alt=""></div>
        <div class="img p-5"><img src="../assets/perusahaan/cikara.png" alt=""></div>
        <div class="img p-5"><img src="../assets/perusahaan/agate.png" alt=""></div>
        <div class="img p-5"><img src="../assets/perusahaan/ahm.png" alt=""></div>
        <div class="img p-5"><img src="../assets/perusahaan/inovindo.png" alt=""></div>
        <div class="img p-5"><img src="../assets/perusahaan/semesta.png" alt=""></div>
        <div class="img p-5"><img src="../assets/perusahaan/skyline.png" alt=""></div>
        <div class="img p-5"><img src="../assets/perusahaan/cikara.png" alt=""></div>
      </div>
    </div>
  </div>

</template>
<style scoped>
.video-wrapper {
    position: relative;
    width: 100%;
    padding-bottom: 56.25%;
    overflow: hidden;
    align-content: center;
  }

  .video-wrapper iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height:100%;
  }
.berita-scroll img{
  height:200px;
}
.content .col-6:hover {
  transform: scale(1.1);
}

.scroll-container {
  overflow: hidden;
  white-space: nowrap;
  position: relative;
  height: 200px;
}

.scroll-content {
  display: flex;
  animation: scroll 5s linear infinite;
}

.scroll-content .img {
  flex: none;
  margin-right: 20px;
}

.scroll-content .img img {
  height: 80px;
  width: auto;
}

* {
  text-decoration: none;
}

.judul-berita {
  color: black;
}

@keyframes scroll {
  0% {
    transform: translateX(0);
  }

  100% {
    transform: translateX(-100%);
  }
}

@media (max-width: 768px) {
.berita-scroll img{
 height: 70px;
}
  .scroll-container {
    overflow: hidden;
    white-space: nowrap;
    position: relative;
    height: 100px;
  }

  .scroll-content .img img {
    height: 30px;
  }

  .scroll-content .img {
    flex: none;
    margin-right: 2px;
  }

  p {
    font-size: 9px;
  }

  .sambutan {
    text-align: center;
  }

  .sambutan p {
    text-align: start;
  }

  @keyframes scroll {
    0% {
      transform: translateX(0);
    }

    100% {
      transform: translateX(-300%);
    }
  }
}
</style>
<script setup>
useHead({ title: "Home" })
const supabase = useSupabaseClient()
const berita = ref([])

const getBerita = async () => {
  const { data, error } = await supabase
    .from('berita')
    .select('*')
  if (error) {
    console.error(error)
  } else {
    berita.value = data
  }
}

onMounted(() => {
  getBerita()
})
</script>
