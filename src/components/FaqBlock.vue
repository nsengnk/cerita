<script setup>
import { ref } from "vue";
import { ArrowDown, ArrowUp } from "@element-plus/icons-vue";

const mask = ref(true);

const maskBlockFaq = () => {
  mask.value = !mask.value;
};

const props = defineProps(["textHeader", "textMain"]);
</script>

<template>
  <div class="col-lg-4"></div>
  <div class="col-lg-4 faq-block">
    <header>
      <div class="row">
        <div class="col-lg-10">{{ props.textHeader }}</div>
        <div class="col-lg-2">
          <el-button
            v-if="mask"
            class="bouton-faq"
            @click="maskBlockFaq"
            :icon="ArrowDown"
          >
          </el-button>
          <el-button
            v-else
            class="bouton-faq"
            @click="maskBlockFaq"
            :icon="ArrowUp"
          >
          </el-button>
        </div>
      </div>
    </header>
    <main v-if="mask">
      {{ props.textMain }}
    </main>
  </div>
  <div class="col-lg-4"></div>
</template>

<style scoped>
.faq-block {
  border: 1px solid lightgray;
  padding: 0px;
  border-radius: 3px;
  margin-top: 1%;
}
.faq-block > header {
  background-color: whitesmoke;
  padding: 2%;
  padding-bottom: 2%;
}
.faq-block > main {
  padding: 2%;
}
.bouton-faq {
  background-color: transparent;
  border: none;
  font-size: 20px;
  outline: none;
}
</style>
