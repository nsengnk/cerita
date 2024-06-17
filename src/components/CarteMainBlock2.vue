<script setup>
import { ref } from "vue";
import { ArrowLeft, ArrowRight } from "@element-plus/icons-vue";

const props = defineProps(["texte"]);
</script>

<template>
  <p>Tapez ici!</p>
  <p class="texte">{{ props.texte }}</p>
</template>

<style scoped>
.texte {
  color: #798da3;
  font-size: 16px;
}
</style>
