<template>
  <h2>{{ message }}</h2>
  <input v-model="message" debounce="500">
</template>

<script>
export default {
  data () {
    return {
      message: 'Change me'
    }
  },
  methods: {
    reverseGreeting () {
      this.message = this.message.split('').reverse().join('')
    }
  }
}
</script>