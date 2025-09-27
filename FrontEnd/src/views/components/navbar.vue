<template>
    <nav>
        <div>
            <ul>
                <li><router-link to="/">Шийдлүүд</router-link> </li>
                <li><router-link to="/">Үнийн санал</router-link> </li>
                <li><router-link to="/">Бидний тухай</router-link> </li>
                <li><router-link to="/">Холбогдох</router-link> </li>
            </ul>
        </div>
        <router-link to="/login">
            <button>Нэвтрэх</button>
        </router-link>
    </nav>
</template>

<script>
import { RouterLink } from 'vue-router';

export default {
    name: "Navbar",
};
</script>

<style scoped>
ul{
    list-style-type: none;
    margin: 0;
    padding: 0;
    overflow: hidden;
}

li{
    float: left;
}

ul li {
  display: block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}
</style>