<template>
  <footer :class="`${!hideBGCOLOR ? 'sub-bg' : ''}`">
    <div class="container">
      <div class="row d-flex align-items-center justify-content-between">
        <div class="col-lg-4">
          <div class="item md-mb50">
            <div class="title">
              <h5>Bize Ulaşın</h5>
            </div>
            <ul>
              <li>
                <span class="icon pe-7s-map-marker"></span>
                <div class="cont">
                  <h6>Address</h6>
                  <p>Gebze/Kocaeli - Bilişim Vadisi</p>
                </div>
              </li>
              <li>
                <span class="icon pe-7s-mail"></span>
                <div class="cont">
                  <h6>Email</h6>
                  <p>akka_1234@hotmail.com</p>
                </div>
              </li>
              <li>
                <span class="icon pe-7s-call"></span>
                <div class="cont">
                  <h6>Telefon</h6>
                  <p>+905399333637</p>
                </div>
              </li>
            </ul>
          </div>
        </div>
        <div class="col-lg-4">
          <div class="item">
            <div class="logo">
              <img src="/img/logo-light.png" alt="logo" />
            </div>
            <div class="social">
              <NuxtLink to="#0">
                <i class="fab fa-facebook-f"></i>
              </NuxtLink>
              <NuxtLink to="#0">
                <i class="fab fa-twitter"></i>
              </NuxtLink>
              <NuxtLink to="#0">
                <i class="fab fa-instagram"></i>
              </NuxtLink>
              <NuxtLink to="#0">
                <i class="fab fa-youtube"></i>
              </NuxtLink>
            </div>
            <div class="copy-right">
              <p>
                © 2023, Portfolıo Template.
                <a href="https://ittyazilim.com">copyright @ kadirkilic.net</a>
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
    props: ['hideBGCOLOR']
};
</script>

<style scoped>
</style>
