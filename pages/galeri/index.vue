<template>
  <div class="container-fluid">
    <div class="text-center judul pt-5">
      <h4 class="text-secondary pt-5">GALERI</h4>
      <h6 class="text-primary">SMKN 4 TASIKMALAYA</h6>
    </div>
    <div class="galeri d-flex justify-content-center">
      <div class="card m-5 shadow rounded-5" style="width: 100%">
        <div class="row p-4 m-3 d-flex justify-content-center">
          <div v-for="(foto, i) in galeri" :key="i" class="col-6 col-md-4 col-lg-3 mb-4">
            <img :src="foto.foto" class="cover" alt="" />
          </div>
          <div v-for="(foto, i) in galeri" :key="i" class="col-6 col-md-4 col-lg-3 mb-4">
            <img :src="foto.foto" class="cover" alt="" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
useHead({ title: "Galeri" })

const supabase = useSupabaseClient()
const galeri = ref([])

const getGaleri = async () => {
  const { data, error } = await supabase
    .from('galeri')
    .select('foto')
  if (error) {
    console.error('Error fetching gallery:', error)
  } else {
    galeri.value = data
  }
}

onMounted(() => {
  getGaleri()
})
</script>

<style scoped>
.cover {
  width: 100%;
  height: 200px;
  object-fit: cover;
  border-radius: 10px;
}
.cover:hover{
  transform: scale(1.1);
}
.card {
  margin: 0 auto;
}

.row {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}

.col-6 {
  padding-left: 0;
  padding-right: 0;
}

@media (min-width: 576px) {
  .col-6 {
    padding-left: 10px;
    padding-right: 10px;
    
  }
}

@media (max-width: 768px) {
  .cover {
    height: 50px;
  }
  .col-6{
    padding-right: 10px;
  }
}

@media (min-width: 992px) {
  .cover {
    height: 200px;
  }
  
}
</style>
