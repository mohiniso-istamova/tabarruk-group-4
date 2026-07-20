<template>
    <div class="flex flex-col justify-between">
        <div class="flex items-center gap-2">
           <div class="bg-[#E64545] p-2 rounded-lg"> 
             <i class="icon-mosque text-xl text-white"></i>
           </div>
            <p class="text-2xl font-medium text-white">175</p>
        </div>
        <p class="mt-4 text-2xl text-[#A7A8AE]">Diqqatga sazovor joylar</p>
    </div>
</template>
<script setup lang="ts">
import {ref, defineProps} from 'vue'

const props = defineProps<{
    title: string
    number: number
    icon: string
}>()

</script>