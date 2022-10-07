<template>
    <div class="flex flex-row">
      <InputWrapper value="High" numberOfQuestionSelected="0"  totalQuestions="14" @click="changeBorderColor" :class="[isActive ? 'border-[#EF5DA8]' : 'border-[#DADBDD]']"/>
    </div>
</template>

<script setup>
import InputWrapper from './components/InputWrapper.vue';
import { ref } from 'vue'
const isActive = ref(false)   
function changeBorderColor(){
  isActive.value = true
} 

</script>
