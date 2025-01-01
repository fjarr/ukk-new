<template>
  <div class="nav bg-dark text-light p-2 d-flex justify-content-center">
    <a href="https://www.instagram.com/smkn4tsmofficial/"><i class="bi bi-instagram m-2"></i></a>
    <a href="https://www.facebook.com/4smkn/?locale=id_ID"> <i class="bi bi-facebook m-2"></i></a>
    <a href="https://x.com/smkn4tsm"><i class="bi bi-twitter-x m-2"></i></a>
    <a href="https://www.youtube.com/channel/UC9WmS4sPok-9bAmRF1ZXrrg"><i class="bi bi-youtube m-2"></i></a>
  </div>

  <nav class="navbar navbar-expand-lg bg-light navbar-light shadow py-4 d-flex justify-content-center">
    <img src="~/assets/kemdikbud.png" alt="">
    <img src="~/assets/jabar.png" alt="">
    <img src="~/assets/smk.png" alt="" class="me-3">
    <div class="c">
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavDropdown"
        aria-controls="navbarNavDropdown" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse px-5" id="navbarNavDropdown">
        <ul class="navbar-nav mx-5 pt-2">
          <li class="nav-item">
            <nuxt-link to="/">
            <h6>HOME</h6>
          </nuxt-link>
          </li>
          <li class="nav-item dropdown mx-3">
            <h6 class=" dropdown-toggle"  id="navbarDropdownMenuLink" role="button" data-bs-toggle="dropdown"
              aria-expanded="false">
              PROFILE
            </h6>
            <ul class="dropdown-menu text-dark" aria-labelledby="navbarDropdownMenuLink">
              <li><nuxt-link to="/profile/sejarah/"><div class="dropdown-item" >Sejarah & Identitas</div></nuxt-link></li>
              <li><nuxt-link to="/profile/visi/"><div class="dropdown-item" >Visi,Misi & Tujuan</div></nuxt-link></li>
              <li><nuxt-link to="/profile/struktur/"><div class="dropdown-item" >Struktur Organisasi</div></nuxt-link></li>
            </ul>
          </li>
          <li class="nav-item mx-3">
            <nuxt-link to="/eskul">
            <h6>EKSTRAKULIKULER</h6>
          </nuxt-link>
          </li>
          <li class="nav-item mx-3">
            <nuxt-link to="/galeri">
            <h6>GALERI</h6>
          </nuxt-link>
          </li>
        </ul>
      </div>
    </div>
  </nav>

</template>
<style scoped>
img {
  height: 50px;
  margin-left: 10px;
}

li {
  font-family: sans-serif;
}
  *{
  text-decoration: none;
  color: black;
  
}
.navbar{
  position: sticky;
  top: 0;
  z-index:1;
}
</style>