<template>
  <div class="home">
    <main-banner/>

    <section id="profile">
      <div class="container">
        <div class="profile-text-wrapper">
          <div class="profile-img-wrapper">
            <div class="bg-frame"></div>
            <img class="profile-img" src="../assets/images/profile-img.jpg" alt="">
            <h2 class="profile-headline">Mathias <span>Jacobsen</span></h2>
          </div>
          <div class="profile-text"  data-sal="slide-left" data-sal-delay="300" data-sal-duration="800" data-sal-easing="ease-out-bounce">
            <p class="main-text">Hej mit navn er Mathias jeg er 23år, og står på springbrættet til at starte min karrier, som <span class="uppercase-highlight">Frontend</span> Udvikler. Jeg er uddannet Multimediedesigner, og har stor passion for både design og <span class="uppercase-highlight">programmering</span>. Jeg læser PBA Web Development på UCL (Odense), og er netop igang med mit 2.Semester, hvor jeg søger en <span class="uppercase-highlight">prakrtikplads</span> til det afsluttende 3.Semester.</p>
          </div>
        </div>
      </div>
    </section>

    <main-slider/>

    <section id="skills">
      <div class="container">
        <div class="row align-items-center">
          <div class="col-12 col-md-10 col-lg-6 col-xl-6 competence" data-sal="slide-right" data-sal-delay="300" data-sal-duration="800" data-sal-easing="ease-out-bounce">
            <h2 class="headline-dot">Kompetencer</h2>
            <p class="main-text"> Min tekniske værktøjskasse råder over forskellige programmer, samt værktøjer som bliver anvendt i forbindelse med udviklingsprocessen af hjemmesider. Jeg har blandt andet arbejdet med CMS systemet Wordpress, samt Umbraco. Det seneste værktøj, som jeg har kastet mig over at lærer er Frameworket Vue.js, samt app sproget Swift til ios development, da jeg finder app udvikling spændende. </p>
            <a href="CvMathias.pdf" target="_blank" class="link-underline">Download mit CV <i class="fas fa-download"></i></a>
          </div>
          <div class="col-12 col-md-9 col-lg-6 col-xl-6 mx-auto" data-sal="slide-left" data-sal-delay="300" data-sal-duration="800" data-sal-easing="ease-out-bounce">
            <img src="../assets/images/kompetencer.png" alt="">
          </div>
        </div>
        <div class="skills-wrapper">
          <div class="img-wrapper">
            <img class="img-filter" src="../assets/images/projectimg.jpg" alt="">
            <div class="img-overlay"></div>
          </div>
          <div class="skills-text-wrapper" data-sal="slide-up" data-sal-delay="300" data-sal-duration="800" data-sal-easing="ease-out-bounce">
            <div class="headline-bg-wrapper">
              <h2 class="main-headline">Fokus på <span>udvikling</span></h2>
            </div>
            <div class="headline-bg-wrapper">
              <h2 class="headline-dot">og detaljeret design</h2>
            </div>
            <p class="main-text">I forbindelse med min uddannelse, som multimediedesigner har jeg arbejdet en del med design, samt udvikling af UX og UI til den rette end user.</p>
          </div>
        </div>
      </div>
    </section>

    <main-footer/>
  </div>
</template>

<script>
// @ is an alias to /src
import MainBanner from "@/components/MainBanner.vue";
import MainSlider from "@/components/MainSlider";
import MainFooter from '@/components/MainFooter.vue';
import sal from "sal.js";

export default {
  name: "home",
  components: {
    MainBanner,
    MainSlider,
    MainFooter
  },
 mounted() {
    sal();
  }
};
</script>


