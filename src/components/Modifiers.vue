<template>
  Input here: <input @keyup.enter="submit">
  <hr>
</template>

<script>
export default {
  methods: {
    submit: function () {
      alert('submitted!')
    }
  }
}
</script>