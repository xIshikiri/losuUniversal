<script setup>
  import maszynaVue from './components/maszyna.vue';
  import sectionMachineVue from './components/sectionMachine.vue';
  import sectionEditVue from './components/sectionEdit.vue';
  import sectionInfoVue from './components/sectionInfo.vue';
  import sectionFooterVue from './components/sectionFooter.vue';
</script>
<template>
  <section class="bodyALL">
    <div class="sectionMachine">
      <sectionMachineVue/>
    </div>

    <div class="sectionEdit">
      <sectionEditVue/>
    </div>

    <div class="sectionInfo">
      <sectionInfoVue/>
    </div>

    <div class="sectionFooter">
      <sectionFooterVue/>
    </div>
  </section>
  

</template>
<style scoped>
  .bodyALL{
    width: 100vw;
    height: auto;
    display: flex;
    align-items: center;
    flex-direction: column;
    overflow-x:hidden;
    flex-wrap: wrap;
  }
  .sectionMachine{
    width: 100vw;
    height: 100vh;
    background-color: blueviolet;
    display: flex;
    align-items: center;
    flex-direction: column;
  }

  .sectionEdit{
    width: 100vw;
    height: 90vh;
    background-color: aquamarine;
    display: flex;
    align-items: center;
    flex-direction: column;
  }

  .sectionInfo{
    width: 100vw;
    height: 80vh;
    background-color: blueviolet;
    display: flex;
    align-items: center;
    flex-direction: column;
  }

  .sectionFooter{
    width: 100vw;
    height: 20vh;
    background-color: aquamarine;
    display: grid;
    place-items: center;
  }
</style>
