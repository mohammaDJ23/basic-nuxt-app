<template>
  <div>
    <div>hi user with id: {{ $route.params.id }}</div>
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

  // this a nuxt method before render the page
  // for validation some data like params and quries
  // you should return boolean

  validate(data) {
    return +data.params.id > 0 && +data.params.id < 101
  },
}
</script>
