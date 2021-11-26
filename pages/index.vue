<template>
  <div>
    {{ x }}
    {{ y }}
  </div>
</template>

<script>
import { defineComponent } from '@nuxtjs/composition-api'
import { useMouse  } from '@vueuse/core'

export default defineComponent({
  setup() {
    return {
      ...useMouse()
    }
  }
})
</script>
