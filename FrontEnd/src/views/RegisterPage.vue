<template>
    <div class="register">
        <h2>Create an Account</h2>
        <form @submit.prevent="handleRegister">
            <input v-model="name" type="text" placeholder="Name" required />
            <input v-model="email" type="email" placeholder="Email" required />
            <input v-model="password" type="password" placeholder="Password" required />
            <button type="submit">Register</button>
        </form>
        <router-link to="/">← Back to Home</router-link>
    </div>
</template>

<script setup>
import { ref } from 'vue'

const name = ref('')
const email = ref('')
const password = ref('')

function handleRegister() {
    console.log('User registered:', { name: name.value, email: email.value, password: password.value })
    alert(`Thanks for registering, ${name.value}!`)
}
</script>

<style scoped>
.register {
    max-width: 400px;
    margin: 100px auto;
    padding: 20px;
    border: 1px solid #ddd;
    border-radius: 8px;
}

input {
    display: block;
    width: 100%;
    margin-bottom: 10px;
    padding: 8px;
}

button {
    width: 100%;
    padding: 10px;
    background: #42b983;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}

button:hover {
    background: #369b70;
}
</style>
