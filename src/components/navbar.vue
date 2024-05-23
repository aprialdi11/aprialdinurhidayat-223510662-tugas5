<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg-primary"> <!-- Menggunakan warna latar belakang yang menarik -->
    <div class="container-fluid"> <!-- Menggunakan container-fluid untuk navbar yang full width -->
      <a class="navbar-brand" href="#">Music Shop</a>
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ml-auto">
          <li class="nav-item">
            <a class="nav-link" href="#">Home</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Produk</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Tentang Kami</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Kontak</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'Navbar'
}
</script>

<style scoped>
.navbar {
  padding: 1rem 0;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1); /* shadow navbar */
  font-family: 'Roboto Condensed', sans-serif; /* Menggunakan jenis font Roboto Condensed */
}

.navbar-brand {
  font-size: 1.75rem;
  font-weight: bold;
  color: #fff; /* Warna font putih */
}

.navbar-nav {
  display: flex;
  align-items: center;
}

.navbar-nav .nav-item {
  margin-left: 1rem;
  margin-bottom: 0; /* Menghapus margin bottom */
  border-radius: 5px; /* Tambahkan sudut bulat */
}

.navbar-nav .nav-link {
  font-size: 1rem;
  transition: color 0.3s ease;
  padding: 0.5rem 1rem; /* Tambahkan padding untuk meningkatkan keterbacaan */
  color: #fff; /* Warna font putih */
}

.navbar-nav .nav-link:hover {
  color: rgba(255, 255, 255, 0.8); /* warna teks link saat hover */
}

.navbar-toggler {
  border: none;
}

.navbar-toggler-icon {
  background-color: rgba(255, 255, 255, 0.8);
  padding: 0.25rem;
  border-radius: 5px;
}

@media (max-width: 992px) {
  .navbar-nav {
    background-color: rgba(255, 255, 255, 0.8);
    padding: 1rem;
    border-radius: 5px;
    width: 100%;
  }

  .navbar-nav .nav-item {
    margin-left: 0;
    margin-bottom: 0.5rem; /* Menambahkan margin bottom pada mobile */
    text-align: center;
  }

  .navbar-nav .nav-link {
    font-size: 1.2rem;
    color: #fff; /* warna teks link pada mobile */
  }
}

/* gaya tambahan */
.navbar-toggler-icon:hover {
  background-color: rgba(255, 255, 255, 1);
  transform: scale(1.1); /* Perbesar icon saat hover */
}
</style>
