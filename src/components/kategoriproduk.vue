<template>
    <div class="q-pa-md">
      <div class="row q-col-gutter-md">
        <div class="col-12 text-h5 q-mb-md">Kategori Produk</div>
        <div class="col-6 col-md-3 col-sm-6" v-for="category in categories" :key="category.id">
          <q-card class="cursor-pointer" @click="navigateToCategory(category.slug)">
            <q-img
              :src="category.image"
              spinner-color="primary"
              spinner-size="82px"
              class="rounded-borders"
              style="height: 150px"
            >
              <div class="absolute-bottom text-subtitle2 text-center bg-transparent">
                {{ category.name }}
              </div>
            </q-img>
          </q-card>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        categories: [
          {
            id: 1,
            name: 'NEW BALANCE',
            slug: 'pakaian',
            image: 'https://i.pinimg.com/originals/27/38/8d/27388d7d86e3cdc65f8279d4d94e4bbc.png'
          },
          {
            id: 2,
            name: 'NIKE YANG KELASS',
            slug: 'elektronik',
            image: 'https://th.bing.com/th/id/OIP.bjxSrwxJiwG1ZHoFJTpzXAHaEc?rs=1&pid=ImgDetMain'
          },
          {
            id: 3,
            name: 'ADIDAS',
            slug: 'olahraga',
            image: 'https://th.bing.com/th/id/OIP.Drp-pANKpa1IITDirZ0i_gHaEo?rs=1&pid=ImgDetMain'
          },
          {
            id: 4,
            name: 'NIKE',
            slug: 'kecantikan',
            image: 'https://th.bing.com/th/id/OIP.pn67rVlEhKrJpdGeA6wJsgHaE7?rs=1&pid=ImgDetMain'
          }
        ]
      }
    },
    methods: {
      navigateToCategory(slug) {
        // tambahkan logika untuk navigasi ke halaman kategori
        console.log(`Navigasi ke kategori ${slug}`)
      }
    }
  }
  </script>