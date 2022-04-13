<!-- the name of this file should be user becuase it is the parent of all user pages -->

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
