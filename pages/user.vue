<template>
  <div>
    <!-- this part is going to run in all user pages -->
    <div>The Root of the user pages</div>

    <!-- the user pages are showing in here -->
    <nuxt-child></nuxt-child>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
}
</script>
