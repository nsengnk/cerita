<script setup>
import { ref } from "vue";
import { ArrowLeft, ArrowRight } from "@element-plus/icons-vue";
import { Bar, Pie, Line } from "vue-chartjs";
import {
  Chart as ChartJS,
  Title,
  Tooltip,
  Legend,
  BarElement,
  CategoryScale,
  LinearScale,
  ArcElement,
  PointElement,
  LineElement,
} from "chart.js";

ChartJS.register(
  Title,
  Tooltip,
  Legend,
  BarElement,
  CategoryScale,
  LinearScale,
  ArcElement,
  PointElement,
  LineElement
);

const histogram_data = {
  labels: ["", "", "", "", ""],
  datasets: [
    {
      label: "Statistiques",
      data: [20, 10, 50, 20, 48, 14],
      backgroundColor: [
        "#08519c",
        "#6baed6",
        "#2175b5",
        "#4292c6",
        "#deebf7",
        "rgba(255, 159, 64, 0.2)",
      ],
      //   borderColor: ["gray", "gray", "gray", "gray", "gray", "gray"],
      //   borderWidth: 1,
    },
  ],
};
const histogram_options = {
  scales: {
    y: {
      beginAtZero: true,
    },
  },
};
const line_options = {
  scales: {
    y: {
      beginAtZero: true,
    },
  },
  responsive: true,
  maintainAspectRatio: false,
};
const line_data = {
  labels: ["January", "February", "March", "April", "May", "June", "July"],
  datasets: [
    {
      label: "Series 1",
      data: [20, 60, 50, 20, 58, 14],
      borderColor: "#08519c",
      borderWidth: 1,
    },
    {
      label: "Series 2",
      data: [5, 10, 12, 25, 48, 17],
      borderColor: "#6baed6",
      borderWidth: 1,
    },
    {
      label: "Series 3",
      data: [15, 18, 22, 45, 8, 7],
      borderColor: "#deebf7",
      borderWidth: 1,
    },
  ],
};
</script>

<template>
  <div class="row main-block-3">
    <div class="col-lg-12">
      <center>
        <h2>Découvrez le palmarès 2023 de la digitilisation au Gabon</h2>
      </center>
    </div>
    <div class="col-lg-2"></div>
    <div class="col-lg-4 graphs">
      <Bar
        style="padding-top: 5%"
        :data="histogram_data"
        :options="histogram_options"
      />
    </div>
    <div class="col-lg-4 graphs">
      <Line :data="line_data" :options="line_options" />
    </div>
  </div>
  <div class="col-lg-2"></div>
</template>

<style scoped>
.main-block-3 {
  padding-top: 2%;
  border-top: 1px solid lightgray;
}
.graphs {
  padding: 2%;
}
</style>
