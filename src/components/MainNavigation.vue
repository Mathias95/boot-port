<template>
    <nav class="nav-menu animated fadeIn">
        <div class="d-flex justify-content-between align-items-center container-fluid p-0">
            <router-link to="/" class="logo">Logo</router-link>
            <Slide right>
            <ul class="mobile-menu">
                <li><a class="nav-link-hover" href="#profile">Profil</a></li>
                <li><a class="nav-link-hover" href="#projects">Portfolio</a></li>
                <li><a class="nav-link-hover" href="#skills">Kompetencer</a></li>
                <li><a class="nav-link-hover" href="#contact">Skab kontakt</a></li>
            </ul>
            </Slide>
            <div class="nav-elements">
                <ul>
                    <li><a class="nav-link-hover" href="#profile">Profil</a></li>
                    <li><a class="nav-link-hover" href="#projects">Portfolio</a></li>
                    <li><a class="nav-link-hover" href="#skills">Kompetencer</a></li>
                    <li><a class="nav-link-hover" href="#contact">Skab kontakt</a></li>
                </ul>
            </div>
        </div>
    </nav>
</template>

<script>
import { Slide } from "vue-burger-menu";
export default {
  name: 'MainNavigation',
  components: {
    Slide
  },
  mounted(){
      let anchorlinks = document.querySelectorAll('a[href^="#"]')
 
    for (let item of anchorlinks) { // relitere 
        item.addEventListener('click', (e)=> {
            let hashval = item.getAttribute('href')
            let target = document.querySelector(hashval)
            target.scrollIntoView({
                behavior: 'smooth',
                block: 'start'
            })
            history.pushState(null, null, hashval)
            e.preventDefault()
        })
    }
  }
};
</script>