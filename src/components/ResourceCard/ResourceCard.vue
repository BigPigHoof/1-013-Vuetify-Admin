<template>
  <v-card width="400" title="管理数量">
    <template v-slot:text>
      <div class="text-h4">10个</div>
      <div class="text-body-2">
        <span class="mr-4">完成：40</span>
        <span class="mr-4">运行中：10</span>
        <span>失败：2</span>
      </div>
      <div class="d-flex" style="height: 12px">
        <div class="bg-blue-darken-2 h-100" style="width: 76%"></div>
        <div class="bg-green-darken-2 h-100" style="width: 20%"></div>
        <div class="bg-red-darken-2 h-100" style="width: 4%"></div>
      </div> </template
  ></v-card>
</template>
<script setup>
// import { computed } from 'vue';
//  const props=defineProps({
//   title: {
//     type: String,
//     default:'管理数量'
//   },
//   normal:{
//     type: Number,
//   },
//   unusual:{
//     type: Number,
//   },
//   fail:{
//     type: Number,
//   }
// });
// const count=computed(()=>{
//   return props?.normal+props?.unusual+props?.fail
// })
</script>
