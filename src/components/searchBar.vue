<template>

<div class="flex flex-row justify-end w-full pb-[20px] pr-[100px] mt-10 ">

<div class="flex flex-row mt-5 justify-center elevation-4  bg-white">

 <input v-model="searchTerm" type="search" name="" placeholder="Search Request" id="" class="focus:outline-none text-bold  p-3 w-[200px]">
 <div class="flex flex-col  justify-center bg-blue-lighten-2 items-center p-3  hover:cursor-pointer" @click="search"><v-icon class="text-white">mdi-magnify</v-icon></div>
</div>

</div>




</template>



<script setup>
import { ref, computed, defineProps } from 'vue'
import { storeToRefs } from 'pinia';
import { useRequestsStore } from '../stores/request';



var {searchTerm} = storeToRefs(useRequestsStore())
var {search} = useRequestsStore()





</script>