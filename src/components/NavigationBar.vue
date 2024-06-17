<script setup>
import { ref } from "vue";
import { Search } from "@element-plus/icons-vue";

const recherche_nav_bar = ref("");
</script>

<template>
  <div class="row nav-bar">
    <div class="col-lg-12 text-left options-navigations">
      <el-menu
        :default-active="activeIndex"
        class="el-menu-demo"
        mode="horizontal"
      >
        <el-menu-item index="0"
          ><img
            src="@/assets/images/LogoCERITA.png"
            style="width: 40%"
            alt="Logo CERITA"
        /></el-menu-item>
        <el-menu-item class="nav-items" index="1">Accueil</el-menu-item>
        <el-menu-item class="nav-items" index="2">Publications</el-menu-item>
        <el-menu-item class="nav-items" index="3"
          >Qui sommes nous?</el-menu-item
        >
        <el-menu-item class="nav-items" index="4">Contacts</el-menu-item>
        <el-menu-item index="5"
          ><el-input
            v-model="recherche_nav_bar"
            style="width: 240px"
            placeholder="Recherche"
            :prefix-icon="Search"
        /></el-menu-item>
        <el-menu-item index="6"
          ><el-button class="buton-faire-don"
            >FAIRE UN DON</el-button
          ></el-menu-item
        >
      </el-menu>
    </div>
  </div>
</template>

<style scoped>
.nav-bar {
  padding: 2%;
  padding-bottom: 0%;
}
.options-navigations {
  padding-top: 2%;
}
.nav-items {
  font-size: 20px;
}
.buton-faire-don {
  background-color: #004aad;
  color: white;
}
.el-menu-demo {
  border: 1px sol;
}
</style>
