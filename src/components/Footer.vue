<template>
  <q-footer class="bg-primary text-white q-pa-md">
    <q-page-container>
      <div class="footer-content">
        <div class="footer-section">
          <q-avatar size="56px" class="q-mb-sm">
            <img src="https://cdn.quasar.dev/logo/svg/quasar-logo.svg">
          </q-avatar>
          <div class="footer-title">Toko Online</div>
          <div class="footer-subtitle">Produk berkualitas dengan harga terbaik</div>
        </div>
        <div class="footer-section">
          <div class="footer-title">Hubungi Kami</div>
          <q-list>
            <q-item>
              <q-item-section avatar>
                <q-icon name="phone" />
              </q-item-section>
              <q-item-section>+62 123 4567 890</q-item-section>
            </q-item>
            <q-item>
              <q-item-section avatar>
                <q-icon name="email" />
              </q-item-section>
              <q-item-section>info@tokoonline.com</q-item-section>
            </q-item>
            <q-item>
              <q-item-section avatar>
                <q-icon name="location_on" />
              </q-item-section>
              <q-item-section>Jl. Contoh Alamat No. 123, Jakarta</q-item-section>
            </q-item>
          </q-list>
        </div>
        <div class="footer-section">
          <div class="footer-title">Ikuti Kami</div>
          <div class="social-icons">
            <q-btn round color="white" text-color="primary" icon="facebook" />
            <q-btn round color="white" text-color="primary" icon="twitter" />
            <q-btn round color="white" text-color="primary" icon="instagram" />
            <q-btn round color="white" text-color="primary" icon="linkedin" />
          </div>
        </div>
      </div>
    </q-page-container>
  </q-footer>
</template>

<script>
export default {
  name: 'Footer'
}
</script>

<style scoped>
.footer-content {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  align-items: flex-start;
}

.footer-section {
  flex: 1;
  min-width: 200px;
  margin: 10px;
}

.footer-title {
  font-size: 18px;
  font-weight: bold;
  margin-bottom: 10px;
}

.footer-subtitle {
  font-size: 14px;
  margin-bottom: 20px;
}

.social-icons {
  display: flex;
  gap: 10px;
}
</style>
