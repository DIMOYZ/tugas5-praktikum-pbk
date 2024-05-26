<template>
    <div class="q-pa-md">
      <div class="row">
        <div class="col-12 text-h5 q-mb-md">Cara Pembelian</div>
        <div class="col-12">
          <q-stepper v-model="step" vertical color="primary" animated>
            <q-step :name="1" title="Pilih Produk" icon="shopping_cart" :done="step > 1">
              Pilih produk yang ingin Anda beli dari daftar produk kami.
            </q-step>
  
            <q-step :name="2" title="Masukkan Keranjang" icon="add_shopping_cart" :done="step > 2">
              Masukkan produk yang Anda inginkan ke dalam keranjang belanja.
            </q-step>
  
            <q-step :name="3" title="Checkout" icon="payment" :done="step > 3">
              Lanjutkan ke halaman checkout untuk melakukan pembayaran.
            </q-step>
  
            <q-step :name="4" title="Konfirmasi Pembayaran" icon="done_all" :done="step > 4">
              Lakukan pembayaran sesuai dengan metode pembayaran yang Anda pilih. Pesanan akan diproses setelah pembayaran dikonfirmasi.
            </q-step>
          </q-stepper>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        step: 1
      }
    }
  }
  </script>