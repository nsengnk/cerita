<script setup>
import { ref } from "vue";
import { ArrowLeft, ArrowRight } from "@element-plus/icons-vue";

const recherche_nav_bar = ref("");
const is_bouton_visible = ref(false);

const afficheBoutonSlides = () => {
  is_bouton_visible.value = !is_bouton_visible.value;
};
const masqueBoutonSlides = () => {
  is_bouton_visible.value = !is_bouton_visible.value;
};
</script>

<template>
  <div
    class="row main-block-1"
    @mouseover="afficheBoutonSlides"
    @mouseout="masqueBoutonSlides"
  >
    <div class="col-lg-2">
      <el-button
        v-show="is_bouton_visible"
        class="bouton-slides-pagination"
        type="info"
        :icon="ArrowLeft"
      ></el-button>
    </div>
    <div class="col-lg-6" style="padding: 8%">
      <p class="main-block1-text1">
        55% des entreprises publiques <br />
        n'ont pas de sites internet!
      </p>
      <p class="main-block1-text2">
        Découvrez notre dernières étude sur la digitilisation des entreprises et
        institutions gabonaises!
      </p>
      <el-button class="buton-lire-article">LIRE L'ARTICLE</el-button>
    </div>
    <div class="col-lg-2 text-left">
      <img
        src="@/assets/images/Batiment_ANINF.png"
        style="width: 100%"
        alt="logo cerita"
      />
    </div>
    <div class="col-lg-2">
      <el-button
        v-show="is_bouton_visible"
        class="bouton-slides-pagination"
        type="info"
        :icon="ArrowRight"
      ></el-button>
    </div>
  </div>
</template>

<style scoped>
.main-block-1 {
  padding-left: 2%;
  padding-right: 2%;
  background-color: whitesmoke;
}
.bouton-slides-pagination {
  background-color: transparent;
  font-size: 100px;
  border: none;
  color: black;
  margin-top: 70%;
}
.main-block1-text1 {
  font-size: 40px;
  color: #004aad;
}
.main-block1-text2 {
  font-size: 18px;
}
.buton-lire-article {
  background-color: #004aad;
  color: white;
}
</style>
