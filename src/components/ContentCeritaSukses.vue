<script setup>
import { ref } from 'vue'

import img1 from '@/assets/cerita/img-1.png';
import img2 from '@/assets/cerita/img-2.png';
import img3 from '@/assets/cerita/img-3.png';

const stories = ref([
    {
        id: 0,
        img: img1,
        name: "Syhabudin Ahmad",
        job: "Project Manager Solutionlabs",
        story: "Program SISTEM top markotop. Selama belajar cara penyampaian dan arahan mentor unik selain itu mentor juga siap membantu kami jika ada kesulitan."
    },
    {
        id: 1,
        img: img2,
        name: "Annastasya KW",
        job: "Project Manager Solutionlabs",
        story: "Dulu sebelum belajar tentang PM di SISTEM sering kesulitan buat manage project. Setelah ikut bootcamp SISTEM jadi tau gimana biar project itu bisa selesai dan achive."
    },
    {
        id: 2,
        img: img3,
        name: "Tasya WA",
        job: "Quality Assurance Solutions",
        story: "Kemarin waktu belajar coding di sini enak banget. Kita di kelas bener-bener dibimbing dari nol (0) sama mentor dari pembelajarannya juga gampang dipahami."
    }
])
</script>

<template>
    <div class="container">
        <div class="title">
            <h2>Cerita Sukses Peserta</h2>
            <p>Cari berbagai macam event teknologi terbaik yang diadakan oleh komunitas dan didukung oleh banyak
                perusahaan besar lainnya</p>
        </div>
        <div class="stories">
            <div v-for="story in stories" :key="story.id" class="story">
                <div class="story__title">
                    <img :src="story.img" :alt="story.name">
                    <div class="name__job">
                        <h3>{{ story.name }}</h3>
                        <p>{{ story.job }}</p>
                    </div>
                </div>
                <p>{{ story.story }}</p>
            </div>
        </div>
    </div>
</template>

<style scoped>
.container {
    display: flex;
    flex-direction: column;
    gap: 10px;
}

.title {
    text-align: center;
}

.title h2 {
    font-family: 'Montserrat';
    font-size: 36px;
    font-weight: 600;
    line-height: 40px;
    letter-spacing: -1px;
    text-align: center;
    margin-bottom: 10px;
}

.title p {
    font-family: 'Inter';
    font-size: 16px;
    font-weight: 400;
    line-height: 28px;
    text-align: center;
}

.stories {
    display: flex;
    flex-direction: row;
    gap: 20px;
}

.story {
    display: flex;
    flex-direction: column;
    gap: 30px;
    align-items: center;
    justify-content: center;
    padding: 25px;
    box-shadow: 0px 30px 70px #000F3821
}

.story p {
    font-family: 'Manrope';
    font-size: 16px;
    font-weight: 400;
    line-height: 27.2px;
    text-align: left;

}

.story__title {
    display: flex;
    gap: 15px;
}

.story__title h3 {
    font-family: 'Manrope';
    font-size: 20px;
    font-weight: 800;
    line-height: 22px;
    text-align: left;
}

.story__title p {
    font-family: 'Manrope';
    font-size: 14px;
    font-weight: 400;
    line-height: 28px;
    text-align: left;

}

.story__title img {
    border-radius: 50%;
}
</style>