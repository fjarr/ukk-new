<template>
    <div class="container-fluid">
        <h4 class="text-center text-primary mt-3">KOMPETENSI KEAHLIAN</h4>
        <h5 class="text-center text-secondary">SMKN 4 TASIKMALAYA</h5>
        <div class="row p-5">
            <div v-for="(foto, i) in jurusan" :key="i" class="col-12">
                <h5 class="ps-5 pt-5">{{ foto.nama }}</h5>
                <h6 class="ps-5">{{ foto.sub }}</h6>
                <div class="card">
                <div class="row">
                    <div class="col-md-5  d-flex flex-row">
                        <div class="p-2"><img :src="foto.foto" alt=""></div>
                        <div class="p-2"><img :src="foto.baju" alt=""></div>
                    </div>
                    <div class="col-md-6">
                        <div class="p-2">{{ foto.deskripsi }}</div>
                    </div>
                </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script setup>
useHead({ title: "Kompetensi Keahlian" })
const supabase = useSupabaseClient()
const jurusan = ref([])

const getJurusan = async () => {
    const { data, error } = await supabase
        .from('jurusan')
        .select('*')
    if (error) {
        console.error(error)
    } else {
        jurusan.value = data
    }
}

onMounted(() => {
    getJurusan()
})
</script>
<style scoped>
img {
    width: 100%;
}

@media (max-width: 768px) {
    .col-md-6 {
        text-align: center;
    }
}
</style>