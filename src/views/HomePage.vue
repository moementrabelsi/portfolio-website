<template>
    <body>
    <div class="header">
<div class="container">
<nav>
    <img src="../assets/images/logo.png" class="logo">
    <ul>
      <li><router-link to="/" exact class="nav-link active">Home</router-link></li>
      <li><router-link to="/about" class="nav-link">About</router-link></li>
      <li><router-link to="/services" class="nav-link">Services</router-link></li>
      <li><router-link to="/portfolio" class="nav-link">Portfolio</router-link></li>
      <li><router-link to="/contact" class="nav-link">Contact</router-link></li>
    </ul>
</nav>
<div class="home-text">
    <p>Fullstack Web Developer</p>
    <h1>Hi, I'm <span>Moemen</span><br>A Software Architecture</h1>
</div>
</div>
    </div>
</body>
</template>

<script>
export default {
  name: "HomePage",
};
</script>
