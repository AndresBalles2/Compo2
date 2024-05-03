<script setup>

import { ref } from 'vue'

let counter = ref(0)

function add() {
    console.log(counter.value++)
}

</script>

<template>
    <div class="bg-blue-500 select-none rounded-lg py-1 px-2 items-center max-w-40 text-center m-auto text-white hover:cursor-pointer hover:bg-white hover:text-blue-500"
    @click="add" >
        Número de clics: {{ counter }}
    </div>
</template>