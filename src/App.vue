<template>
  <div id="app">
    <Verification />
  </div>
</template>

<script>
import Verification from './components/Verification.vue'

export default {
  name: "App",
  components: {
    Verification
  },
  data: () => ({
    doc: {},
    itens : [
    {}
    ],
    item: {}
  })
};
</script>

