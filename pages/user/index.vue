<template>
  <div>
    <div>hi all users</div>
    <div><button @click="onClick">back to home</button></div>
  </div>
</template>

<script>
export default {
  name: 'User',
  methods: {
    onClick() {
      this.$router.push('/')
    },
  },
}
</script>
