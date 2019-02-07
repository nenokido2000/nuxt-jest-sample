<template>
  <div>
    <p>{{ status ? 'on' : 'off'}}</p>
    <button @click="handleClick">toggle</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      status: false
    }
  },
  methods: {
    handleClick() {
      this.status = !this.status
    }
  }
}
</script>

<style scoped>

</style>
