<template>
  <section class="contact-sec section-padding position-re">
    <div class="container">
      <div class="row justify-content-center">
        <div class="col-lg-8 col-md-10">
          <div class="sec-head text-center">
            <h6 class="wow fadeIn" data-wow-delay=".5s">Bize Ulaşın</h6>
            <h3 class="wow color-font">
              Gelin İletişime Geçelim Ve Birlikte Sihir Yapalım.
            </h3>
          </div>
        </div>
      </div>
      <div class="row justify-content-center">
        <div class="col-lg-10">
          <div class="form wow fadeInUp" data-wow-delay=".5s">
            <form id="contact-form">
              <div class="messages"></div>
              <div class="controls">
                <div class="row">
                  <div class="col-lg-4">
                    <div class="form-group">
                      <input
                        id="form_name"
                        type="text"
                        name="name"
                        placeholder="İsim"
                        required="required"
                      />
                    </div>
                  </div>
                  <div class="col-lg-4">
                    <div class="form-group">
                      <input
                        id="form_email"
                        type="email"
                        name="email"
                        placeholder="Email"
                        required="required"
                      />
                    </div>
                  </div>
                  <div class="col-lg-4">
                    <div class="form-group">
                      <input
                        id="form_name"
                        type="text"
                        name="name"
                        placeholder="Soyisim"
                        required="required"
                      />
                    </div>
                  </div>
                  <div class="col-12">
                    <div class="form-group">
                      <textarea
                        id="form_message"
                        name="message"
                        placeholder="Mesajınız"
                        rows="4"
                        required="required"
                      ></textarea>
                    </div>
                  </div>
                  <div class="col-12">
                    <div class="text-center">
                      <NuxtLink to="#0" class="butn bord curve mt-30">
                        <span>Mesajı Gönder</span>
                      </NuxtLink>
                    </div>
                  </div>
                </div>
              </div>
            </form>
          </div>
        </div>
      </div>
    </div>
    <div v-if="!noLine" class="line bottom left"></div>
  </section>
</template>

<script>
export default {
  props: ["noLine"],
};
</script>

<style scoped>
</style>
