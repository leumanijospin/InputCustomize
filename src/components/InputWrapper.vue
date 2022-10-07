<template>
    <div class="flex flex-row w-[256.3px] h-[38px] bg-white border-[0.47px] border-solid border-[#919FAF] rounded-lg p-[10px] bg-white mx-auto mt-8 relative">
        <input type="radio" id="value" name="difficulty" :value="value" class="accent-[#EF5DA8]">
            <div class="not-italic font-light text-sm leading-[18px] text-[#919FAF] w-[50px] h-[18px] font-['Outfit']">
                <label for="value" class="pl-2">{{ value }}</label>
               <label for="value" class="pl-[155px]">{{ numberOfQuestionSelected }}/{{ totalQuestions}}</label>
            </div>
   </div>
</template>

<script setup>
defineProps({
    value: {
        type: String,
        required: true
    },
    numberOfQuestionSelected: {
        type: Number,
        required: true
    },
    totalQuestions: {
        type: Number,
        required: true
    }
    
  })
  
</script>
