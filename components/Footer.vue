<template>
    <div class="container-fluid">
        <div class="row pt-5 px-5 text-light bg-dark">
            <div class="col-12 col-md-4">
                <h4>Hubungi Kami</h4>
                <hr>
                <h6>SMKN 4 Tasikmalaya</h6>
                <p>Jl Depok Kel. Sukamenak Kec. Purbaratu Kota Tasikmalaya 46196.</p>
                <i class="bi bi-telephone"> +62-265-3120-53</i><br>
                <i class="bi bi-envelope"> info@smkn4-tsm.sch.id</i>
            </div>
            <div class="col-12 col-md-4">
                <h4>Media Sosial</h4>
                <hr>
                <i class="bi bi-facebook"><a href="https://www.facebook.com/4smkn/?locale=id_ID"> Facebook</a></i><br>
                <i class="bi bi-youtube"><a href="https://www.youtube.com/channel/UC9WmS4sPok-9bAmRF1ZXrrg"> Youtube</a>
                </i><br>
                <i class="bi bi-instagram"><a href="https://www.instagram.com/smkn4tsmofficial/"> Instagram</a> </i><br>
                <i class="bi bi-twitter-x"><a href="https://x.com/smkn4tsm"> Twitter</a></i>
            </div>
            <div class="col-12 col-md-4">
                <h4>Link Eksternal</h4>
                <hr>
                <a href="https://www.kemdikbud.go.id/">Kemdikbud</a><br>
                <a href="#">Dapodikdas</a><br>
                <a href="https://psmk.jabarprov.go.id/">PSMK</a><br>
                <a href="https://disdik.jabarprov.go.id/">Disdik Jabar</a>
                <hr>
                <p>@smkn4tsm. All rights reserved <br><span>Designed and Engineered by fjarr</span></p>
            </div>
        </div>
    </div>
    <div class="map bg-dark px-5 pb-5">
            <iframe
                src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3957.2131636317317!2d108.25189907411307!3d-7.3299399720880825!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2e6f59eeb6bda36f%3A0xa9e724a275da6c2d!2sSMK%20Negeri%204%20Tasikmalaya!5e0!3m2!1sid!2sid!4v1735726981056!5m2!1sid!2sid"
                width="100%" height="auto" style="border:0;" loading="lazy"
                referrerpolicy="no-referrer-when-downgrade"></iframe>
        </div>
</template>

<style scoped>
a {
    text-decoration: none;
    color: white;
}

i a {
    text-decoration: none;
    color: white;
}

@media (max-width: 768px) {
    a {
        font-size: 12px;
    }

    h6 {
        font-size: 14px;
    }

    p {
        font-size: 12px;
    }

    .bi {
        font-size: 12px;
    }

    .container-fluid .row .col-4 h4 {
        font-size: 14px;
    }
}

@media (min-width: 768px) {
    .container-fluid .row .col-md-4 h4 {
        font-size: 16px;
    }

    .container-fluid .row .col-md-4 h6 {
        font-size: 14px;
    }

    .container-fluid .row .col-md-4 p {
        font-size: 14px;
    }

    .bi {
        font-size: 16px;
    }
}
</style>
