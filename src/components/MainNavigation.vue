<template>
    <nav class="nav-menu">
        <div class="d-flex justify-content-between align-items-center container-fluid p-0">
            <router-link to="/" class="logo">Logo text</router-link>
            <Slide right>
            <ul class="mobile-menu">
                <li><a class="nav-link-hover" href="#">Forside</a></li>
                <li><a class="nav-link-hover" href="#">Profil</a></li>
                <li><a class="nav-link-hover" href="#">Portfolio</a></li>
                <li><a class="nav-link-hover" href="#">Skab kontakt</a></li>
            </ul>
            </Slide>
            <div class="nav-elements">
                <ul>
                    <li><a class="nav-link-hover" href="#">Forside</a></li>
                    <li><a class="nav-link-hover" href="#">Profil</a></li>
                    <li><a class="nav-link-hover" href="#">Portfolio</a></li>
                    <li><a class="nav-link-hover" href="#">Skab kontakt</a></li>
                </ul>
            </div>
        </div>
    </nav>
</template>

<script>
import { Slide } from "vue-burger-menu";
export default {
  name: "MainNavigation",
  components: {
    Slide
  }
};
</script>