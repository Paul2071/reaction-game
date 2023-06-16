<template>
  <h1>Reaction time</h1>
  <button @click="start"> Click to play </button>
</template>

<script>


export default {
  name: 'App',
  components: {  },
  data() {
    return {
      isPlaying: false,
      
    }
  },
  methods: {
    start() {
      this.isPlaying = true
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #444;
  margin-top: 60px;
}
</style>
