<template>
  <div>
    <Navbar ref="navbar" />
    <FreelancreIntro id="anasayfa" />
    <Services5 id="ozelliklerim" />
<!--    <Works5 id="portfolıo" />-->
    <AboutUs5 id="yetenekler" />
<!--    <FullTestimonials showHead />-->
<!--    <Blogs2 />-->
    <SContactForm noLine id="bizeulasin" />
    <Footer />
  </div>
</template>

<script>
import Navbar from "~/components/Navbar/index.vue";
import FreelancreIntro from "~/components/Freelancre-intro/index.vue";
import Services5 from "~/components/Services5/index.vue";
import Works5 from "~/components/Works5/index.vue";
import AboutUs5 from "~/components/About-us5/index.vue";
// import FullTestimonials from "~/components/Full-testimonials/index.vue";
// import Blogs2 from "~/components/Blogs2/index.vue";
import SContactForm from "~/components/S-contact-form/index.vue";
import Footer from "~/components/Footer/index.vue";
export default {
  layout: "dark",
  components: {
    Navbar,
    FreelancreIntro,
    Services5,
    // Works5,
    AboutUs5,
    // FullTestimonials,
    // Blogs2,
    SContactForm,
    Footer,
  },
  head() {
    return {
      titleTemplate: '%s - Freelancer Dark'
    };
  },
  mounted() {
    var navbar = this.$refs.navbar.$el;
    if (window.pageYOffset > 300) {
      navbar.classList.add("nav-scroll");
    } else {
      navbar.classList.remove("nav-scroll");
    }
    window.addEventListener("scroll", () => {
      if (window.pageYOffset > 300) {
        navbar.classList.add("nav-scroll");
      } else {
        navbar.classList.remove("nav-scroll");
      }
    });
  },
};
</script>

<style>
html {
  scroll-behavior: smooth;
}
</style>
