<template>
    <div class="register">
        <h2>Create an Account</h2>
        <form @submit.prevent="handleLogin">
            <input v-model="name" type="text" placeholder="Name" required />
            <input v-model="email" type="email" placeholder="Email" required />
            <input v-model="password" type="password" placeholder="Password" required />
            <button type="submit">Register</button>
        </form>
        <router-link to="/">← Back to Home</router-link>
    </div>
</template>

<script>
    
</script>