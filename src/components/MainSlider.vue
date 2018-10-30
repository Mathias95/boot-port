<template>
    <section id="projects">
      <div class="container">
        <div class="row">
            <div class="col-12 col-md-9 col-lg-6 col-xl-5 projects-text-wrapper">
            <h2 class="headline-dot">Seneste projekter</h2>
            <p class="main-text">Lorem ipsum dolor sit amet, consectetur adipiscing eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
            </div>
        </div>
      </div>
      <div class="main-carousel"
        data-flickity='{ "freeScroll": true }'>
            <div class="carousel-cell">

            </div>
            <div class="carousel-cell">
                
            </div>
            <div class="carousel-cell"></div>
            <div class="carousel-cell"></div>
            <div class="carousel-cell"></div>
        </div>
        <div class="container">
            <a class="button button-main-btn" href="#">Flere projekter<img src="../assets/images/arrow-right.png" alt=""></a>
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
                // any options from Flickity can be used
            }
            }
        }
    };
</script>
