<template>
  <div>
    <input type="text" :value="userId" @input="onInput" />
    <button @click="navigateUser">load the user</button>
  </div>
</template>

<script>
export default {
  name: 'UserInput',
  data() {
    return {
      userId: '',
    }
  },
  methods: {
    onInput(event) {
      this.userId = event.target.value
    },
    navigateUser() {
      this.$router.push(`/user/${this.userId}`)
    },
  },
}
</script>
