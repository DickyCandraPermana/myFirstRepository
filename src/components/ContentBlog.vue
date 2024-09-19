<script setup>
import { ref } from "vue";

import img1 from "@/assets/blog/img1.png";
import img2 from "@/assets/blog/img2.png";
import img3 from "@/assets/blog/img3.png";
import img4 from "@/assets/blog/img4.png";
import profile from "@/assets/blog/profile_pict.png";

const events = ref([
    {
        id: 0,
        url: img1,
        title: "Quality Assurance",
        jenisKelas: "Live Class",
        durasi: "3 Bulan",
        peminat: {
            url: profile,
            peminat: "3000+"
        }
    },
    {
        id: 1,
        url: img2,
        title: "Project Manager",
        jenisKelas: "Live Class",
        durasi: "3 Bulan",
        peminat: {
            url: profile,
            peminat: "3000+"
        }
    },
    {
        id: 2,
        url: img3,
        title: "Development Operational",
        jenisKelas: "Live Class",
        durasi: "3 Bulan",
        peminat: {
            url: profile,
            peminat: "3000+"
        }
    },
    {
        id: 3,
        url: img4,
        title: "Fullstack Developer",
        jenisKelas: "Live Class",
        durasi: "3 Bulan",
        peminat: {
            url: profile,
            peminat: "3000+"
        }
    }
])

</script>

<template>
    <div class="blog">
        <h2>Pilih Pengalaman Event Terbaik</h2>
        <p>
            Cari berbagai macam event teknologi terbaik yang diadakan oleh komunitas dan di dukung
            oleh banyak perusahaan besar lainnya
        </p>
        <div class="cards">
            <div v-for="event in events" :key="event.id" class="card">
                <div class="card_img">
                    <img :src="event.url" :alt="event.title">
                </div>
                <div class="card_caption">
                    <div class="card__caption__title">
                        <h4>{{ event.title }}</h4>
                        <p>{{ event.jenisKelas }} {{ event.durasi }}</p>
                    </div>
                    <div class="card__caption__peminat">
                        <img :src="event.peminat.url" :alt="event.peminat.peminat">
                        <p>{{ event.peminat.peminat }}</p>
                    </div>
                    <a href="#">Daftar Sekarang →</a>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.blog h2 {
    font-family: 'Montserrat';
    font-size: 32px;
    font-weight: 600;
    line-height: 64px;
    letter-spacing: -2px;
    text-align: center;
}

.blog p {
    font-family: Inter;
    font-size: 16px;
    font-weight: 400;
    line-height: 28px;
    text-align: center;
}

.cards {
    display: flex;
    justify-content: space-around;
}

.card {
    width: 23%;
    display: flex;
    flex-direction: column;
    box-shadow: 2px 4px 4px rgba(0, 0, 0, 0.2);
}

.card .card_img img {
    width: 100%;
}

.card .card_caption {
    display: flex;
    flex-direction: column;
    gap: 10px;
    padding: 12px;
}

.card__caption__title p {
    text-align: left;
}

.card__caption__title h4 {
    font-family: 'Montserrat';
    font-size: 1.2em;
}

.card__caption__peminat {
    display: flex;
    align-items: start;
    gap: 10px;
}
</style>