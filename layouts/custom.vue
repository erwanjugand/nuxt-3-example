<template>
  <div>
    <Head>
      <Title>{{ title }}</Title>
    </Head>
    <header>
      <slot name="header" />
    </header>

    <main>
      <slot />
    </main>

    <footer>
      <slot name="footer" />
    </footer>
  </div>
</template>

<style lang="css">
main {
  background: red;
}
</style>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  props: {
    title: String
  }
})
</script>
