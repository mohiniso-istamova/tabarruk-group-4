<template>
  <div class="pt-40 bg-[#0b0e1a] min-h-screen px-10">
    <div class="grid grid-cols-1 md:grid-cols-[1fr_2fr] gap-6 max-w-6xl mx-auto items-stretch">
      
      <CStatisticCard
        v-for="item in statsData"
        :key="item.id"
        :item="item"
      />

    </div>
  </div>
</template>

<script setup>

import CStatisticCard from '@/components/Cards/CStatisticCard.vue';

const statsData = [
  {
    id: 1,
    value: "175",
    label: "Diqqatga sazovor joylar",
    iconName: "mosque",
    hasDivider: false
  },
  {
    id: 2,
    value: "37 mln",
    label: "Aholi soni",
    iconName: "earth-globe", 
    hasDivider: true // Vertikal chiziq chiqishi uchun 
  }
];
</script>