<template>
  <button @click="onClick()" :style="{ background: color }" class="btn">{{ text }}</button>
</template>

<script lang="ts">
import { defineComponent } from "@vue/runtime-core";

  export default defineComponent({
    name: "Button",
    props: {
      text: String,
      color: String,
    },
    methods: {
      onClick() {
        console.log("click");
        
      }
    },
  })
</script>