<template>
  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="card-columns">
          <div class="card" v-for="product in products" :key="product.id">
            <img :src="product.image" class="card-img-top" :alt="product.title">
            <div class="card-body">
              <h5 class="card-title">{{ product.title }}</h5>
              <p class="card-text">{{ product.description }}</p>
              <p class="card-price">{{ product.price }}</p>
              <a href="#" class="btn btn-primary">Beli Sekarang</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'CardSection',
  data() {
    return {
      products: [
        {
          id: 1,
          title: 'Gitar Akustik',
          description: 'Gitar akustik dengan suara yang jernih dan desain klasik.',
          price: 'Rp 1.500.000',
          image: 'https://hlsmusicindonesia.com/wp-content/uploads/2022/11/ad880ce-nat-web.jpg' // Update with the correct image path
        },
        {
          id: 2,
          title: 'Piano Elektrik',
          description: 'Piano elektrik dengan berbagai fitur modern.',
          price: 'Rp 5.000.000',
          image: 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSNz0p1CFjijoYXIUMKntXtMNltgfmtjTdsSTNJA02BFg&s' // Update with the correct image path
        },
        {
          id: 3,
          title: 'Drum Set',
          description: 'Set drum lengkap untuk pemula hingga profesional.',
          price: 'Rp 3.000.000',
          image: 'https://id.yamaha.com/id/files/PHX_PWH_f_0001_with-shadow__25dc2b1254808a51aca02a22fe71922d.jpg?impolicy=resize&imwid=396&imhei=396' // Update with the correct image path
        },
        {
          id: 4,
          title: 'Biola',
          description: 'Biola dengan kualitas suara yang memukau.',
          price: 'Rp 2.000.000',
          image: 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR6LwYH5hB-1xu2n66kKZsSin82vQQuej09GrWbMoiQlA&s' // Update with the correct image path
        },
        {
          id: 5,
          title: 'Saxophone',
          description: 'Saxophone dengan desain elegan dan suara merdu.',
          price: 'Rp 4.000.000',
          image: 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTdOjGP5tXaqggLS-9NejzMuGYGMLRlyWACKPGdcjLdTg&s' // Update with the correct image path
        },
        {
          id: 6,
          title: 'Keyboard',
          description: 'Keyboard dengan berbagai macam suara dan ritme.',
          price: 'Rp 2.500.000',
          image: 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ_Og9OCe8k4qh73w0UvNQaWTSzh-OZ9U8U4G4FRflfTQ&s' // Update with the correct image path
        }
      ]
    };
  }
};
</script>

<style scoped>
.card-columns {
  column-count: 3; /* Mengatur tiga kolom */
  column-gap: 1rem; /* Jarak antara kartu-kartu */
}

.card {
  display: inline-block;
  width: 100%;
  margin-bottom: 1rem; /* Jarak antara kartu-kartu */
  border: none;
  border-radius: 15px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.card:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
}

.card img {
  border-top-left-radius: 15px;
  border-top-right-radius: 15px;
  object-fit: cover; /* Mengatur gambar agar sesuai proporsi */
  height: 200px; /* Atur ketinggian gambar */
  width: 100%; /* Gambar mengisi lebar kartu */
}

.card-body {
  padding: 20px;
}

.card-title {
  font-size: 1.2rem;
  font-weight: bold;
  color: #333;
  margin-bottom: 10px;
}

.card-text {
  font-size: 1rem;
  color: #555;
  margin-bottom: 15px;
}

.card-price {
  font-size: 1rem;
  color: #007bff;
  font-weight: bold;
  margin-bottom: 15px;
}

.btn {
  background-color: #007bff;
  color: #fff;
  border: none;
  border-radius: 5px;
  padding: 10px 20px;
  text-decoration: none;
  transition: background-color 0.3s ease;
}

.btn:hover {
  background-color: #0056b3;
}
</style>
