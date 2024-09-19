<script setup>

</script>

<template>
    <div class="about-us">
        <div class="bar">
            <div class="white"></div>
            <div class="yellow"></div>
            <div class="blue"></div>
        </div>
        <div class="aboutus__container">
            <article class="kotak">
                <h4>TENTANG KAMI</h4>
                <h3>Mulai Karir Sukses Anda di Teknik Perangkat Lunak dengan SISTEM BOOTCAMP</h3>
                <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Pariatur odio beatae
                    iste nobis quasi provident nulla nisi non, velit est. Qui tempora dolorum
                    ex corporis itaque magni reprehenderit optio dolores?</p>
            </article>
            <article class="kotak">
                <h4>MISI KAMI</h4>
                <h3>Membuat Peradaban Teknologi yang Terbaik untuk seluruh dunia</h3>
                <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Pariatur odio beatae
                    iste nobis quasi provident nulla nisi non, velit est. Qui tempora dolorum
                    ex corporis itaque magni reprehenderit optio dolores?</p>
            </article>
        </div>
    </div>
</template>

<style scoped>
.bar {
    height: 25px;
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 0;
}

.bar .white {
    width: 25%;
    height: 100%;
    background-color: white;
}

.bar .yellow {
    width: 50%;
    height: 100%;
    background-color: #FACA15;
}

.bar .blue {
    width: 25%;
    height: 100%;
    background-color: #0D28A6;
}

.aboutus__container {
    background-color: #F4F0F8;
    padding: 80px;
    display: flex;
    justify-content: space-between;
    gap: 50px;
}

.aboutus__container h4 {
    font-family: 'Inter';
    font-size: 16px;
    font-weight: 600;
    line-height: 20px;
    letter-spacing: 3px;
    text-align: left;
}

.aboutus__container h3 {
    font-family: 'Montserrat';
    font-size: 24px;
    font-weight: 600;
    line-height: 40px;
    letter-spacing: -1px;
    text-align: left;
}

.aboutus__container p {
    font-family: 'Inter';
    font-size: 16px;
    font-weight: 400;
    line-height: 28px;
    text-align: left;
}
</style>