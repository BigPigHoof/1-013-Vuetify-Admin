<template>
  <v-table>
    <thead>
      <tr>
        <th v-for="item in columns" :key="item.name" class="text-left">
          {{ item.label }}
        </th>
      </tr>
    </thead>
    <tbody>
      <tr v-for="(item, index) in dataSource" :key="item[rowKey]">
        <td v-for="column in columns" :key="column.name">
          <slot
            v-if="column.slotName"
            :name="column.slotName"
            v-bind="{ row: item, index }"
          ></slot>
          <template v-else>
            {{ item[column.name] }}
          </template>
        </td>
      </tr>
    </tbody>
  </v-table>
</template>
<script setup>
defineProps({
  columns: {
    type: Array,
  },
  dataSource: {
    type: Array,
  },
  rowKey: { type: String, default: "id" },
});
</script>
