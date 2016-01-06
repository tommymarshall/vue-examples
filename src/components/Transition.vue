<template>
  <div v-if="show" transition="potato">{{ text }}</div>
  <button v-model="show" v-on:click="toggleShow">Toggle show</button>
</template>

<script>
export default {
  data () {
    return {
      show: false,
      text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Totam odio tenetur velit voluptate quasi amet consequuntur cupiditate harum perspiciatis quibusdam odit.'
    }
  },
  methods: {
    toggleShow () {
      this.show = !this.show
    }
  }
}
</script>

<style>
.potato-transition {
  transition: all .3s ease;
  height: 30px;
  padding: 10px;
  background-color: #eee;
  overflow: hidden;
}

.potato-enter, .potato-leave {
  height: 0;
  padding: 0 10px;
  opacity: 0;
}
</style>