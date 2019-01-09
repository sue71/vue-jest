<template>
  <div>
    {{ exclamationMarks }}
    <type-script-child />
  </div>
</template>

<script lang="ts">
import TypeScriptChild from './TypeScriptChild.vue'
import Vue from 'vue'

export default Vue.extend({
  computed: {
    exclamationMarks(): string {
      return 'string'
    }
  },
  components: {
    TypeScriptChild
  }
})
</script>
