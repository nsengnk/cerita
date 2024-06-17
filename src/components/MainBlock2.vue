<script setup>
import { ref } from "vue";
import CarteMainBlock2 from "@/components/CarteMainBlock2.vue";
import { ArrowLeft, ArrowRight } from "@element-plus/icons-vue";
</script>

<template>
  <div class="row" style="padding: 2%">
    <div class="col-lg-12">
      <center>
        <h2>Nos dernières publications</h2>
        <p style="font-size: 18px; color: cadetblue">
          Establish trust with customers by reassuring them that the process is
          quick, simple, and lucrative.
        </p>
      </center>
    </div>
    <div class="col-lg-2"></div>
    <div class="col-lg-2 carte">
      <CarteMainBlock2
        :texte="'Palmarès de la digitilisation des institutions en République Gabonaise'"
      />
    </div>
    <div class="col-lg-1"></div>
    <div class="col-lg-2 carte">
      <CarteMainBlock2
        :texte="'Les modèles de Machine Learning comme leviers de développement de l\'économie'"
      />
    </div>
    <div class="col-lg-1"></div>
    <div class="col-lg-2 carte">
      <CarteMainBlock2
        :texte="'Focus sur la nouvelle stratégie cyber de l\'Etat gabonais'"
      />
    </div>
    <!-- <div class="col-lg-1"></div>
    <div class="col-lg-2 carte"><CarteMainBlock2 /></div>
    <div class="col-lg-1"></div>
    <div class="col-lg-2 carte"><CarteMainBlock2 /></div>
    <div class="col-lg-2"></div> -->
  </div>
</template>

<style scoped>
.carte {
  border: 1px solid lightgray;
  height: 200px;
  padding: 2%;
  border-radius: 5px;
  background-color: white;
}
</style>
