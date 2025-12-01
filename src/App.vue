
<template>
  <nav class="navbar">
    <div class="logo"><img src="./assets/img/table.png" alt=""></div>

    <ul class="links">
    <li><btn Name="À propos" Link=""/></li>
    <li><btn Name="Cursus" Link=""/></li>
    <li><btn Name="Projets" Link=""/></li>
    </ul>
  </nav>

  <ul class="mobile-menu" :class="{ open: isOpen }">
    <li><btn Name="À propos" Link=""/></li>
    <li><btn Name="Cursus" Link=""/></li>
    <li><btn Name="Projets" Link=""/></li>
  </ul>

<section class="hero">
    <div class="hero-content">
      <h2>Bonjour! Je suis</h2>
      <h1>Mathys LEININGER</h1>
      <p>
        Développeur passionné et créatif, je crée des projets web modernes et performants.
        Toujours curieux, j’aime apprendre de nouvelles technologies et relever des défis.
      </p>
    </div>
    <div class="hero">
      <btn Name="Email" Link="#"/>
      <btn Name="GitHub" Link="#"/>
      <btn Name="CV" Link="#"/>
      <btn Name="Arffornia" Link="#"/>
    </div>


  </section>
  
</template>


<script setup>
  import './assets/style.css'

  import { computed,ref } from 'vue';
  import Btn from '../component/btn.vue';

const isOpen = ref(false)

const toggle = () => (isOpen.value = !isOpen.value)
const close = () => (isOpen.value = false)
</script>

