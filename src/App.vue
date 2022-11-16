<script setup>
  import maszynaVue from './components/maszyna.vue';
  import sectionMachineVue from './components/sectionMachine.vue';
</script>
<template>
  <div class="sectionMachine">
    <sectionMachineVue/>
  </div>
  

  <section class="sectionEdit">
    
  </section>

</template>
<style scoped>
  .sectionMachine{
    width: 100vw;
    height: 95vh;
    background-color: blueviolet;
    display: flex;
    align-items: center;
    flex-direction: column;
  }

  .wrapMachine{
    width: 80vw;
    height: 70vh;
    background-color: aquamarine;
  }
</style>
