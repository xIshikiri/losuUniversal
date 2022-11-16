<script setup>
  import maszynaVue from './maszyna.vue';
  import editListCardVue from './editListCard.vue';
</script>
<template>

    <h1>EDYTUJ</h1>
    
    <h4>COMBOBOX PLACE</h4>
    <div class="wrap">
        <div class="listBlock">
          <editListCardVue text1="1" text2="2" text3="3"/>
        </div>
        <div class="listBlock">
          <editListCardVue text1="najlepsze" text2="najgorsze" text3="najdzwniejsze"/>
        </div>
        <div class="listBlock">
          <editListCardVue text1="przegrane" text2="wygrane" text3="kartkówki"/>
        </div>
      
    </div>

    
    

</template>
<style scoped>
  .wrap{
    background-color: blueviolet;
    width: 90vw;
    height: 60vh;
    display: flex;
    align-items: center;
    justify-content: space-evenly;
  }

  .listBlock{
    background-color: beige;
    height: 80%;
    width: 20vw;
    display: flex;
    align-items: center;
    flex-direction: column;
    padding-top: 20px;
  }
</style>
