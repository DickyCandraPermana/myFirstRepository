<script setup>
import IconBrand from '@/components/icons/IconBrand.vue'
</script>

<template>
    <footer>
        <div class="column">
            <i>
                <IconBrand />
            </i>
            <div class="address">
                <h5>Jogja Office</h5>
                <p>Jl. Kresna. Gamping kidul, Amberketawang, Kec.<br />
                    Gamping, Kabupaten Sleman, DIY 55294</p>
            </div>
            <div class="address">
                <h5>Jakarta Office</h5>
                <p>Cibis Nine Building Lantai 11 Jl. TB Simatupang No. <br />
                    2, Jakarta Selatan</p>
            </div>
        </div>
        <div class="column">
            <h2>Bootcamp</h2>
            <ul>
                <li>Devops</li>
                <li>Quality Assurance</li>
                <li>Fullstack Developer</li>
                <li>Project Manager</li>
            </ul>
        </div>
        <div class="column">
            <h2>SISTEM</h2>
            <ul>
                <li>Tentang Kami</li>
                <li>Events</li>
                <li>FAQ</li>
            </ul>
        </div>
        <div class="column">
            <h2>Ikuti Kami</h2>
            <button><img src="@/assets/symbol/Container.png" alt="Instagram"></button>
            <div class="line"><img src="@/assets/symbol/Symbol_1.png" alt="Phone">
                <p>+62 811-269-086</p>
            </div>
            <div class="line"><img src="@/assets/symbol/Symbol.png" alt="Mail">
                <p>putro@solutionlabs.id</p>
            </div>
        </div>
    </footer>
</template>

<style scoped>
footer {
    display: flex;
    justify-content: space-around;
    align-items: start;
    background: #071F51;
    color: #ABB0BA;
    padding: 60px;
}

ul {
    list-style-type: none;
}

li {
    margin: 10px 0;
}

button {
    width: auto;
    height: auto;
    background: none;
    border: none;
}

img {
    width: 20px;
    height: 20px;
}

.line {
    display: flex;
    gap: 15px;
}

h2 {
    font-family: 'Manrope';
    font-size: 24px;
    font-weight: 800;
    line-height: 24px;
    text-align: left;
    color: white;
}

.column {
    display: flex;
    flex-direction: column;
    gap: 20px;
}

.address h5 {
    font-family: 'Manrope';
    font-size: 16px;
    font-weight: 600;
    line-height: 27.2px;
    text-align: left;
}

.address p {
    font-family: 'Manrope';
    font-size: 14px;
    font-weight: 400;
    line-height: 24px;
    text-align: left;
}
</style>