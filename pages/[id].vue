<template>
    <div class="container-fluid">
        <div class="foto p-3  text-center">
            <img :src="berita.foto" alt="foto" style="width:80%;" v-if="berita" />
        </div>
        <div class="content mx-3">
            <h3 >
            {{ berita.judul }}
            </h3>
        </div>
        <div class="tanggal  mx-3">
        <p class="pt-3 pb-5 ">{{ berita.tanggal }}</p>
        </div>
        <div class="content ">
        <p class=" pb-5 mx-3">
        {{ berita.isi }}
        </p>
        </div>
    </div>
</template>

<script setup>
useHead({ title: "berita" })
const supabase = useSupabaseClient();
const berita = ref({});
const route = useRoute();

const getBerita = async () => {
    const { data, error } = await supabase
        .from('berita')
        .select(`*`)
        .eq('id', route.params.id);

    if (data && data.length > 0) {
        berita.value = data[0];
    }
};

onMounted(() => {
    getBerita();
});
</script>
