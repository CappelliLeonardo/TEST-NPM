<script>
export default {
  data() {
    return {
        title: 'Ciao ragazzi'
    };
  },
};
</script>

<template>
    <header>
        <h1>
            {{ title }}
        </h1>
    </header>
</template>

<style scoped>
    h1{
        color: lightcoral;
        text-align: center;
    }
</style>
