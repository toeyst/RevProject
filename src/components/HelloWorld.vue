<script setup>
defineProps({
  msg: {
    type: String,
    required: true
  }
})
</script>

<template>
  <!DOCTYPE html>
  <html>

  <head>
    <title>Shoe Store</title>
    <link rel="stylesheet" type="text/css" href="style.css">
  </head>

  <body>
    <header>
      <h1>Shoe Store</h1>
    </header>
    <nav>
      <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#products">Products</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
    <main>
      <h2 id="home">Welcome to Shoe Store</h2>
      <p>We offer a wide selection of stylish and comfortable shoes for men, women, and children. Take a look at our
        latest arrivals:</p>
      <ul id="products">
        <li>Women's Running Shoes</li>
        <li>Men's Dress Shoes</li>
        <li>Kid's Sneakers</li>
      </ul>
      <h2 id="about">About Us</h2>
      <p>Shoe Store was founded in 2010 with the goal of providing high-quality footwear at affordable prices. Our team
        is dedicated to helping you find the perfect pair of shoes, whether you need them for everyday wear or for a
        special occasion.</p>
      <h2 id="contact">Contact Us</h2>
      <p>If you have any questions or would like to place an order, please don't hesitate to contact us:</p>
      <p>Phone: 555-555-5555</p>
      <p>Email: info@shoestore.com</p>
    </main>
    <footer>
      <p>Copyright Shoe Store 2021</p>
    </footer>
  </body>

  </html>

</template>

<style scoped>
body {
  font-family: Arial, sans-serif;
  color: #333333;
}

header {
  background-color: #f5f5f5;
  padding: 20px;
}

h1 {
  margin: 0;
  text-align: center;
}

nav {
  background-color: #333333;
  color: #ffffff;
}

nav ul {
  list-style: none;
  margin: 0;
  padding: 0;
  display: flex;
}

nav li {
  padding: 20px;
}

nav a {
  color: #ffffff;
  text-decoration: none;
}

main {
  padding: 20px;
}

h2 {
  margin: 0;
}

ul {
  list-style: none;
  margin: 0;
  padding: 0;
}

footer {
  background-color: #f5f5f5;
  padding: 20px;
  text-align: center;
}

h1 {
  font-weight: 500;
  font-size: 2.6rem;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {

  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
