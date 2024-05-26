<template>
    <div class="q-pa-md">
      <div class="row q-col-gutter-md">
        <div class="col-12 text-h5 q-mb-md">Produk Unggulan</div>
        <div class="col-6 col-md-3 col-sm-6" v-for="product in featuredProducts" :key="product.id">
          <q-card class="cursor-pointer" @click="navigateToProduct(product.slug)">
            <q-img
              :src="product.image"
              spinner-color="primary"
              spinner-size="82px"
              class="rounded-borders"
              style="height: 200px"
            />
            <q-card-section>
              <div class="text-subtitle1 text-weight-bold">{{ product.name }}</div>
              <div class="text-caption text-grey">{{ product.category }}</div>
              <div class="text-subtitle2 text-weight-bold q-mt-sm">Rp{{ product.price.toLocaleString() }}</div>
            </q-card-section>
          </q-card>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        featuredProducts: [
          {
            id: 1,
            name: 'Produk 1',
            slug: 'produk-1',
            category: 'Kategori 1',
            price: 99000,
            image: 'https://wallpapercave.com/wp/wp1828091.png' // Memperbarui URL gambar untuk produk pertama
          },
          {
            id: 2,
            name: 'Produk 2',
            slug: 'produk-2',
            category: 'Kategori 2',
            price: 149000,
            image: 'https://c.static-nike.com/a/images/f_auto/w_1920,c_limit/nni8ipthzexjynxjdm8j/1021-homepage-apla-xa.jpg' // Memperbarui URL gambar untuk produk kedua
          },
          {
            id: 3,
            name: 'Produk 3',
            slug: 'produk-3',
            category: 'Kategori 3',
            price: 79000,
            image: 'https://wallpapercave.com/wp/wp1870191.jpg' // Memperbarui URL gambar untuk produk ketiga
          },
          {
            id: 4,
            name: 'Produk 4',
            slug: 'produk-4',
            category: 'Kategori 4',
            price: 129000,
            image: 'https://ceklist.id/wp-content/uploads/2021/07/Sepatu-Futsal-Specs-Terbaik.jpg' // Memperbarui URL gambar untuk produk keempat
          }
        ]
      }
    },
    methods: {
      navigateToProduct(slug) {
        // tambahkan logika untuk navigasi ke halaman produk
        console.log(`Navigasi ke produk ${slug}`)
      }
    }
  }
</script>
