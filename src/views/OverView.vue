<template>
  <v-container>
    <ResourceCard />
    <BasicTable :columns="columns" :dataSource="dataSource" />
  </v-container>
</template>
<script setup>
import ResourceCard from "@/components/ResourceCard";
import BasicTable from "@/components/BasicTable";
const columns = [
  {
    name: "name",
    label: "名称",
  },
  {
    name: "time",
    label: "时间",
  },
];
const dataSource = [
  { id: 1, name: "应用1", time: "2022-01-01 10:10:00" },
  { id: 2, name: "应用2", time: "2022-01-01 10:10:00" },
  { id: 3, name: "应用3", time: "2022-01-01 10:10:00" },
  { id: 4, name: "应用4", time: "2022-01-01 10:10:00" },
  { id: 5, name: "应用5", time: "2022-01-01 10:10:00" },
  { id: 6, name: "应用6", time: "2022-01-01 10:10:00" },
];
</script>
