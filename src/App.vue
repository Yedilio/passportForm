<template>
  <div id="app">
    <PassportForm />
  </div>
</template>

<script>
  import PassportForm from "./components/PassportForm";

  export default {
    name: 'App',
    components: {
      PassportForm,
    }
  }
</script>

<style lang="scss" scoped>
  div {
    height: 100%;
    width: 100%;
    background-color: rgba(34, 34, 34, .9);
    display: flex;
    justify-content: center;
  }
</style>
