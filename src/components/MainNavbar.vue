<script setup>
import IconBrand from '@/components/icons/IconBrand.vue'
</script>

<template>
    <header>
        <i>
            <IconBrand />
        </i>
        <nav>
            <ul>
                <li><a href="">Home</a></li>
                <li><a href="">Blog</a></li>
                <li><a href="">About Us</a></li>
                <li><a href="">Contact Us</a></li>
            </ul>
        </nav>
        <button class="btn btn-primary">Contact Us</button>
    </header>
</template>

<style scoped>
/* header {
    display: block;
    position: sticky;
    top: 0;
    left: 0;
} */
nav ul {
    list-style-type: none;
    display: flex;
    gap: 20px;
    justify-content: space-evenly;
}

nav li a {
    text-decoration: none;
    color: black;
    font-weight: 400;
}

nav li a:hover {
    animation: 1s ease-in-out;
    color: darkgray;
}
</style>