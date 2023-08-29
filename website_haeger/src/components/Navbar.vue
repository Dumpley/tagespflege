<template>
  <header>
    <div class="container">
      <p class="logo">Logo</p>
      <nav>
      <ul>
        <li>
          <router-link to="/">Start</router-link>
        </li>
        <li>
          <router-link to="/about">Info</router-link>
        </li>
        <li>
          <router-link to="/gallery">Galerie</router-link>
        </li>
      </ul>
    </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Navbar'
}
</script>

<style scoped>
  .container {
    width: 80%;
    margin: 0 auto;
  }
  header {
    background: #55d6aa;
  }
  header::after {
    content: '';
    display: table;
    clear: both;
  }
  .logo {
    float: left;
    padding: 10px 0;
  }
  nav {
    float: right;
  }
  nav ul {
    margin: 0;
    padding: 0;
    list-style: none;
  }
  nav li {
    display: inline-block;
    margin-left: 50px;
    padding-top: 25px;
    position: relative;
  }
  nav a {
    color: #444;
    text-decoration: none;
    text-transform: uppercase;
    font-size: 14px;
  }
  nav a::before {
    content: '';
    display: block;
    height: 5px;
    width: 100%;
    background-color: #444;
    position: absolute;
    top: 0;
    width: 0;
    transition: all ease-in-out 200ms;
  }
  nav a:hover {
    color: #000
  }
  nav a:hover::before {
    width: 100%;
  }
</style>