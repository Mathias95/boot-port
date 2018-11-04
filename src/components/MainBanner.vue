<template>
    <div>
        <section class="main-banner target" id="top">
            <div class="empty-circle-big"></div>
            <div class="container animated bounceInUp">
                <div class="wrapper-box">
                    <h1 class="banner-heading">Kreativ<span>Frontender</span></h1>
                    <div class="empty-divider"></div>
                </div>
                <p class="subbanner-heading">Subtitle - Subheadertitle</p>
            </div>
            <div class="container-fuild banner-sub animated fadeInLeft">
                <ul>
                    <li><a href="mailto:mathiasrjacobsen@gmail.com?Subject=Hello%20again"><i class="fas fa-envelope"></i><span>Mail</span></a></li>
                    <li><a href="https://www.facebook.com/mathias.jacobsen3" target="_blank"><i class="fab fa-facebook-square"></i><span>Facebook</span></a></li>
                    <li><a href="https://github.com/Mathias95" target="_blank"><i class="fab fa-github"></i><span>GitHub</span></a></li>
                </ul>
            </div>
        </section>
        <div class="section-slider">
            <ul>
                <li><a href="#top">01</a></li>
                <li><a href="#profile">02</a></li>
                <li><a href="#projects">03</a></li>
                <li><a href="#skills">04</a></li>
                <li><a href="#contact">05</a></li>
            </ul>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'MainBanner'
    };
</script>