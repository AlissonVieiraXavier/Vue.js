<template>
  <div>
    <Nav :navLinks="navLinks" :navConfig="navConfig" :btnConfig="btnConfig">
      <img class="img" src="" alt="" srcset="" /> <!-- A slot For your project Logo -->
    </Nav>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import Nav from 'vue-nav-ui'
export default defineComponent({
    name:"NavBar",
    components: {
        Nav}

})

</script>
