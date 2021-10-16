<template>
  <NuxtLayout name="custom" :title="title">
    <template #header>
      {{ header}}
    </template>
    <h1 v-text="title" />
    <Button>
      Click Me !
    </Button>
  </NuxtLayout>
</template>


<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  layout: false,

  data: () => ({
    header: 'Header',
    title: 'Nuxt 3 app example'
  }),

})
</script>

