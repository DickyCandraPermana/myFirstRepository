<script setup>
import { ref } from 'vue'

import CommentsImage from '@/assets/Comments.svg'
import WeekScheduleImage from '@/assets/Week Schedule.svg'
import PostImage from '@/assets/Post.svg'


const services = ref([
    {
        url: CommentsImage,
        title: 'Build Community'
    },
    {
        url: WeekScheduleImage,
        title: 'Share Event'
    },
    {
        url: PostImage,
        title: 'Get Information'
    }
])
</script>

<template>
    <article>
        <h3>CAREER ACELERATE</h3>
        <h1>Meningkatkan Karir Anda di SISTEM Bootcamp</h1>
        <p>
            Pelajari dari ahli Teknik Perangkat Lunak yang berpengalaman di SEA dan
            mempercepat karir anda sebagai Software Engineer.
        </p>
        <div class="services">
            <div class="service" v-for="service in services" :key="service">
                <div class="icon">
                    <img :src="service.url" :alt="service.title">
                </div>
                <h4>{{ service.title }}</h4>
            </div>
        </div>
        <button class="btn btn-primary">Contact Us</button>
    </article>
</template>

<style scoped>
article {
    width: 616px;
    height: 444px;
    display: flex;
    flex-direction: column;
    gap: 32px;
}

h3 {
    font-weight: 600;
    line-height: 20px;
    letter-spacing: 3px;
    color: #FACA15;
}

h1 {
    font-size: 48px;
    font-weight: 600;
    line-height: 64px;
}

.services {
    display: flex;
    justify-content: space-around;
    font-family: Poppins;
    font-size: 18px;
    font-weight: 600;
    line-height: 27px;
}

.service {
    width: 190px;
    height: 64px;
    display: flex;
    flex-direction: row;
    align-items: center;
    gap: 5px;
}

.service .icon {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 64px;
    height: 64px;
    border-radius: 16px;
    background-color: #075EFD33;
}
</style>