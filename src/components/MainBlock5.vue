<script setup>
import { ref } from "vue";
import FaqBlock from "@/components/FaqBlock.vue";
</script>

<template>
  <div class="row main-block-5">
    <div class="col-lg-12">
      <center>
        <h2>FAQ</h2>
      </center>
    </div>
    <FaqBlock
      :text-header="'Le CERITA est-il un organisme indépendant ?'"
      :text-main="`Lorem ipsum dolor sit amet. Vel corrupti minus et dolor Quis vel aut
      sint ab dolorem magni aut amet vitae! Aut aperiam internos qui internos
      rerum in quibusdam rerum est nemo minus et provident saepe! Vel nisi
      similique ut itaque itaque sit praesentium aliquam ut laboriosam rerum sed
      ipsum nostrum. Sed molestias eligendi sit quod dolor aut enim sequi est`"
    />
    <FaqBlock
      :text-header="'This is a frequently asked question. Ipsum dolor sit amet? '"
    />
    <FaqBlock
      :text-header="'This is a frequently asked question. Ipsum dolor sit amet? '"
    />
  </div>
</template>

<style scoped>
.main-block-5 {
  padding: 2%;
}
</style>
<!-- Lorem ipsum dolor sit amet. Vel corrupti minus et dolor Quis vel autem
      sint ab dolorem magni aut amet vitae! Aut aperiam internos qui internos
      rerum in quibusdam rerum est nemo minus et provident saepe! Vel nisi
      similique ut itaque itaque sit praesentium aliquam ut laboriosam rerum sed
      ipsum nostrum. Sed molestias eligendi sit quod dolor aut enim sequi est -->
