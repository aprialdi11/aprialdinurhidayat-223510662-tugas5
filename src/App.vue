<template>
  <div id="app">
    <Navbar />
    <main>
      <Carousel />
      <div class="container mt-5">
        <CardSection />
      </div>
    </main>
    <Footer />
  </div>
</template>

<script>
import Navbar from './components/navbar.vue';
import Carousel from './components/carousel.vue';
import CardSection from './components/card.vue';
import Footer from './components/footer.vue';

export default {
  components: {
    Navbar,
    Carousel,
    CardSection,
    Footer
  }
}
</script>

<style>
body {
  font-family: 'Arial', sans-serif;
  margin: 0;
  padding: 0;
  background: linear-gradient(135deg, #000000, #ffffff, #9e7b57); /* Gradasi dari hitam ke putih ke coklat */
}

#app {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

main {
  flex: 1;
}

.container {
  max-width: 1200px;
  margin: auto;
}

footer {
  background-color: #343a40;
  color: white;
  padding: 1rem 0;
  text-align: center;
}

a {
  text-decoration: none;
  color: inherit;
}

a:hover {
  text-decoration: underline;
}
</style>
