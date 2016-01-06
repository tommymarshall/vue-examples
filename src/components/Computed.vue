<template>
  <h3>Full name is: {{ firstName }} - {{ fullName }} </h3>
</template>

<script>
export default {
  data () {
    return {
      firstName: 'Tommy',
      lastName: 'Marshall'
    }
  },
  computed: {
    fullName: function () {
      return this.firstName + ' ' + this.lastName
    }
  }
}
</script>