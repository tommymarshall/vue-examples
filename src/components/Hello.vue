<template lang="jade">
  <h1>{{ message }} - {{ heading }}</h1>
  <button v-on:click="reverseMessage">Reverse</button>
  <hr>
</template>

<script>
export default {
  props: ['heading'],
  data () {
    return {
      message: 'Hello World!'
    }
  },
  ready () {
    alert('awesome')
  },
  methods: {
    reverseMessage () {
      this.message = this.message.split('').reverse().join('')
    },

    whatever () {

    }
  }

}
</script>

<style lang="sass?indentedSyntax" scoped>
  h1
    font-family: Helvetica
    color: blue
</style>
