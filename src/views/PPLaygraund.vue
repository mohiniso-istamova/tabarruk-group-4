<template>
 <div class="mt-50">
   <div class=" grid grid-cols-3 container gap-4">
    <CCountryStatisticCard class="bg-gray-600/30 p-6 rounded-xl backdrop-blur-xl"/>
    <div class="col-span-2 grid grid-cols-4 bg-gray-600/30 p-6 rounded-xl backdrop-blur-xl">
      <CCountryStatisticCard class="border-r pr-3 border-white mr-4"  
      v-for="(el, idx) in data.splice(1,1)"
      v-bind="data"
      />
    </div>
  </div>
 </div>
</template>
<script setup lang="ts">
import CCountryStatisticCard from '@/components/Cards/CCountryStatisticCard.vue';
const data = [
  {
    icon: 'icon-mosque',
    number: 175,
    title: 'Diqqatga sazovor joylar'
  },
   {
    icon: 'icon-mosque',
    number: 37,
    title: 'Aholi soni'
  }
]
</script>