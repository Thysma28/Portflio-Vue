<script setup>
import MyPdf from '../src/assets/img/CV.pdf';


const props = defineProps({
  Name: {
    type: String,
    default: "#"
  }
})


</script>

<template>
  <a class="fancy-btn" v-bind:href="MyPdf">
    {{ props.Name }}
  </a>
</template>

<style scoped>

.fancy-btn {
    color: black;
    font-weight: bold;
    padding: 12px 24px;
    border-radius: 12px; /* bords arrondis */
    border: none;
    cursor: pointer;
    transition: transform 0.2s ease, box-shadow 0.2s ease;
    font-size: 16px;
}

.fancy-btn:hover {
    transform: scale(1.05); /* grandit de 5% */
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
}

</style>