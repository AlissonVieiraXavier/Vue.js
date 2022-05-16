<template>
<div>
    <img alt="Vue logo" src="./assets/logo.png">
    <h1> FormVue </h1>  

</div>

</template>

<script lang="ts">
import { defineComponent } from 'vue';


export default defineComponent({
  name: 'App',

});
</script>

<style scoped>
div{
  text-align: center;
  display: flex;
  flex-direction: column;
  align-items: center;

}

img{
  width: 150px;
  max-height: 100px;
}

</style>