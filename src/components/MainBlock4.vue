<script setup>
import { ref } from "vue";
import { ArrowLeft, ArrowRight } from "@element-plus/icons-vue";
</script>

<template>
  <div class="row main-block-4">
    <div class="col-lg-12" style="padding-bottom: 1%">
      <center>
        <h2>Les chiffres de la digitilisation au Gabon</h2>
      </center>
    </div>
    <div class="col-lg-3"></div>
    <div class="col-lg-2 chiffres">
      <center>
        <el-progress type="circle" :percentage="70" />
      </center>
      <center class="description-chiffre">MONTHLY SUBSCRIPTION</center>
    </div>
    <div class="col-lg-2 chiffres">
      <center>
        <el-progress type="circle" :percentage="50" />
      </center>
      <center class="description-chiffre">ANNUAL SUBSCRIPTION</center>
    </div>
    <div class="col-lg-2 chiffres">
      <center>
        <el-progress type="circle" :percentage="30" />
      </center>
      <center class="description-chiffre">REFRESH SUBSCRIPTION</center>
    </div>
    <div class="col-lg-3"></div>
  </div>
</template>

<style scoped>
.main-block-4 {
  padding: 2%;
  background-color: whitesmoke;
}
.description-chiffre {
  font-size: 18px;
  font-weight: bold;
  color: #9fafc1;
}
</style>
