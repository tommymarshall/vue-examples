<template>
  <div id="app">
    <h1>VueJS stuff</h1>
    <Hello heading="Heading"></Hello>
    <Modifiers></Modifiers>
    <Computed></Computed>
    <Todos></Todos>
    <Bindings></Bindings>
    <Model></Model>
    <Transition></Transition>
  </div>
</template>

<script>
import Hello from './components/Hello'
import Modifiers from './components/Modifiers'
import Transition from './components/Transition'
import Bindings from './components/Bindings'
import Computed from './components/Computed'
import Todos from './components/Todos'
import Model from './components/Model'

export default {
  components: {
    Hello,
    Computed,
    Modifiers,
    Todos,
    Bindings,
    Transition,
    Model
  }
}
</script>