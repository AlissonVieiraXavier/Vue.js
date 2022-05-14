<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <olaMundo />
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import olaMundo from "@/components/olaMundo.vue"

export default defineComponent({
  name: 'App',
      components:{
        olaMundo
    }
});
</script>
