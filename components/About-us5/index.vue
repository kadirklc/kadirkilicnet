<template>
  <section class="about-cr">
    <div class="container-fluid">
      <div class="row">
        <div class="col-lg-6 img md-mb50">
          <img src="/img/skills.png" alt="" />
        </div>
        <div class="col-lg-5 valign">
          <div class="cont full-width">
            <h3 class="color-font">Web Yazılım</h3>
            <h5 class="co-tit mb-15">Porjelerinizi geliştiriyoruz.</h5>
            <p>
              Kullandığınız projeleri geliştirme
            </p>
            <div class="skills-box mt-40">
              <div class="skill-item">
                <h5 class="fz-14 mb-15">Front-End Web Development</h5>
                <div class="skill-progress">
                  <div class="progres" data-value="95%"></div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import aboutSkillsProgress from "../../common/aboutSkillsProgress";
export default {
  mounted() {
    aboutSkillsProgress();
  },
};
</script>

<style scoped>
</style>
