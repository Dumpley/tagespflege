<template>
  <div>
    <nav class="mainNavBar">
        <div class="logo">sample</div>
        <ul>
            <li>
                <router-link to="/" class="nav-link">Home</router-link>
            </li>
            <li>
                <router-link to="/about" class="nav-link">About</router-link>
            </li>
        </ul>
    </nav>
  </div>
</template>

<script>
export default {
  name: 'Navbar'
}
</script>

<style scoped>
.mainNavBar {
    display: flex;
    justify-content: space-between;
    padding: 0px 16px;
    width: 100%;
    top: 0px;
    background: #eee;
    transition: background 0.4s;
}

.mainNavBar .logo {
    font-size: xx-large;
    height: 60px;
    text-align: center;
    align-items: center;
}

</style>