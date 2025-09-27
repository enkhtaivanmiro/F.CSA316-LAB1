<template>
    <div class="landing">
        <Navbar/>
        <h1>Welcome to Our App 🚀</h1>
        <p>Join us today and explore amazing features!</p>
        <router-link to="/register">
            <button>Register Now</button>
        </router-link>
    </div>
</template>

<script setup>
import Navbar from './components/navbar.vue';

// no script needed here
</script>

<style scoped>
.landing {
    text-align: center;
}

button {
    padding: 10px 20px;
    background: #42b983;
    color: var(--orange);
    border: none;
    border-radius: 5px;
    cursor: pointer;
}

button:hover {
    background: #369b70;
}
</style>
