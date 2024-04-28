<template>
  <CustomButton/>
  <NativeButton />
</template>

<script>
import CustomButton from './components/CustomButton.vue';
import NativeButton from './components/NativeButton.vue'

export default {
  name: 'App',
  components: {
    CustomButton,
    NativeButton
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
