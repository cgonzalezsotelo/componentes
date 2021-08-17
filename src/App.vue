<template>
  <div>
    <RickAndMorty/>
  </div>
</template>

<script>
import RickAndMorty from './components/RickAndMorty'

export default {
  name: 'App',
  components: {
    RickAndMorty
  }
}
</script>

<style>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
</style>
