<template>
    <main class="columns is-gapless is-multiline">
      <div class="column is-one-quarter">
        <BarraLateral/>
      </div>
      <div class="column is-three-quarter">
       <FormuLario @aoSalvarTarefa="SalvaTarefa"/>
      </div>
      <div class="lista">
        <TarefA v-for="(tarefa,index) in tarefas" :key="index" :tarefa="tarefa"/>
      </div>
    </main>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import BarraLateral from './components/BarraLateral.vue'
import FormuLario from './components/Form.vue'
import TarefA from './components/Tarefa.vue'
import ITarefa from './interfaces/ITarefa';

export default defineComponent({
  name: 'App',
  components: {
    BarraLateral,
    FormuLario,
    TarefA,
  },
  data(){
    return{
     tarefas: [] as ITarefa[]
    }
  },
  methods: {
    SalvaTarefa (tarefa:ITarefa){
      this.tarefas.push(tarefa);

    }
  }
});
</script>

<style>
@media screen and (min-width: 768px){  
  .lista{
    position: relative;
    margin-top: -500px;
    width: 70%;
    left: 27%;
    padding-top:20px;
    }
}

</style>

