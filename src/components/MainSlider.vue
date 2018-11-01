<template>
    <section id="projects">
      <div class="container">
        <div class="row">
            <div class="col-12 col-md-9 col-lg-6 col-xl-5 projects-text-wrapper" data-sal="slide-right" data-sal-delay="300" data-sal-duration="800" data-sal-easing="ease-out-bounce">
            <h2 class="headline-dot">Seneste projekter</h2>
            <p class="main-text">Lorem ipsum dolor sit amet, consectetur adipiscing eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
            </div>
        </div>
      </div>
      <div class="main-carousel"
        data-flickity='{ "freeScroll": true, "pageDots": false, "prevNextButtons": false}'>
            <div class="project-cell p1">
                <div class="project-overlay">
                    <h3 class="project-headline">Mobile<br> App design</h3>
                </div>
            </div>
            <div class="project-cell p2">
                <div class="project-overlay">
                    <h3 class="project-headline">Mobile<br> App design</h3>
                </div>
            </div>
            <div class="project-cell p3">
                <div class="project-overlay">
                    <h3 class="project-headline">Mobile<br> App design</h3>
                </div>
            </div>
            <div class="project-cell p4">
                <div class="project-overlay">
                    <h3 class="project-headline">Mobile<br> App design</h3>
                </div>
            </div>
        </div>
        <div class="container">
            <router-link to="/Projects" class="button button-main-btn">Flere projekter<img src="../assets/images/arrow-right.png" alt=""></router-link>
        </div>
    </section>
</template>

<script>
import Flickity from 'vue-flickity'
    export default {
        name: 'MainSlider',
        components: {
            Flickity
        },
          data () {
            return {
            flickityOptions: {
                initialIndex: 3,
                prevNextButtons: true,
                pageDots: true,
                wrapAround: true,
                freeScroll: true
                }
            }
        }
    };
</script>
