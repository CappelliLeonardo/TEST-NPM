<script>

/*
 Come faccio ad utilizzare un componente dentro ad un altro?
 Si seguono tre passaggi:
 1) importazione nome del file
 2) Dichiarazione del componente all'interno dell'oggetto
 3) Utilizzo del componente
*/

// 1) importazione
import AppHeader from './components/AppHeader.vue';

export default {
  data() {
    return {
        count: 0
    };
  },
  // 2) Dichiarazione dei componenti 
  components: {
    AppHeader
  }

};
</script>

<template>

    <div>
        <!-- 3)Utilizzo del componenete -->
            <AppHeader/>

            <h1>
                Ciao ragazzi
            </h1>
            <p>
                {{ count }}
            </p>
            <button @click="count++">
                Incrementa count
            </button>
    </div>
</template>

<style scoped></style>
