<template>
  <header class="freelancre valign">
    <div class="container">
      <div class="row">
        <div class="col-lg-4">
          <div class="img">
            <img src="/img/foto.jpeg" alt="" />
          </div>
        </div>
        <div class="col-lg-8 valign">
          <div class="cont">
            <h1 class="cd-headline clip">
              Merhaba, Benim adım Kadir, Kodlamayı seviyorum. Front-end alanında profesyonel destek sağlayabilirim
              <span class="cd-words-wrapper">
                <VueTyper
                  :text="['Web software', 'Front-end developer', 'User interface']"
                  :repeat="Infinity"
                  initial-action="erasing"
                  :pre-type-delay="70"
                  :type-delay="70"
                  :pre-erase-delay="2000"
                  :erase-delay="250"
                  erase-style="backspace"
                  caret-animation="smooth"
                  class="color-font fw-600"
                ></VueTyper>
              </span>
            </h1>
          </div>
        </div>
      </div>

      <div class="states">
        <div class="container">
          <ul class="flex">
            <li class="flex">
              <div class="numb valign">
                <h3>2</h3>
              </div>
              <div class="text valign">
                <p>
                  Yıllık <br />
                  Deneyim
                </p>
              </div>
            </li>

            <li class="flex">
              <div class="numb valign">
                <h3>16+</h3>
              </div>
              <div class="text valign">
                <p>
                  Proje tamamlandı <br />
                  Ve teslim edildi
                </p>
              </div>
            </li>

            <li class="mail-us">
              <a href="mailto:akka_1234@hotmail.com?subject=Subject">
                <div class="flex">
                  <div class="text valign">
                    <div class="full-width">
                      <p>Bana temas edin</p>
                      <h6>akka_1234@hotmail.Com</h6>
                    </div>
                  </div>
                  <div class="mail-icon">
                    <div class="icon-box">
                      <span class="icon color-font pe-7s-mail"></span>
                    </div>
                  </div>
                </div>
              </a>
            </li>
          </ul>
        </div>
      </div>
    </div>
    <div class="line bottom left"></div>
  </header>
</template>

<script>
export default {};
</script>

<style>
span.right {
    display: none !important;
}
span.caret:empty:before {
    content: "\200B";
    background: #fff;
    width: 1px;
    height: 100%;
    position: absolute;
    top: 0;
}
</style>
