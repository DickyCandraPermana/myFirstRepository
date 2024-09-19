<script setup>
import { ref } from 'vue'

import img1 from '@/assets/partner/img-1.png';
import img2 from '@/assets/partner/img-2.png';
import img3 from '@/assets/partner/img-3.png';
import img4 from '@/assets/partner/img-4.png';
import img5 from '@/assets/partner/img-5.png';
import img6 from '@/assets/partner/img-6.png';

const partners = ref([
    { id: 0, url: img1 },
    { id: 1, url: img2 },
    { id: 2, url: img3 },
    { id: 3, url: img4 },
    { id: 4, url: img5 },
    { id: 5, url: img6 },
])
</script>

<template>
    <div class="partner">
        <h2>Berbagai Mitra Untuk Mendukung Ekosistem Digital SISTEM</h2>
        <div class="partner__list">
            <div class="partner__item" v-for="partner in partners" :key="partner.id">
                <img :src="partner.url" alt="Partner Logo">
            </div>
        </div>
    </div>
</template>

<style scoped>
h2 {
    font-family: 'Montserrat';
    font-size: 32px;
    font-weight: 600;
    line-height: 64px;
    letter-spacing: -2px;
    text-align: center;
}

.partner {
    display: flex;
    flex-direction: column;
    gap: 50px
}

.partner__list {
    display: flex;
    justify-content: space-around;
    gap: 60px;
}
</style>