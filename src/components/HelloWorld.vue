<script setup>

import endent from "endent";
import { ref } from "vue";


let diagram = ref(endent`graph TD
    if --> then
`);

function nodeClick(node) {
    console.log(node)
}

</script>

<template>
    <div class="content bg-white">
      <vue-mermaid-string :value="diagram" @node-click="nodeClick"/>
    </div>
</template>

<style scoped>

</style>