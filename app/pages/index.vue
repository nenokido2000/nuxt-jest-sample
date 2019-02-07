<template>
  <section class="container">
    <div>
      <h2>カウンター</h2>
      <h3>Count {{ count }}</h3>
      <button type="button" @click="increment">Increment</button>
    </div>
  </section>
</template>

<script>
import { mapGetters, mapActions } from 'vuex'

export default {
  computed: {
    ...mapGetters(['count'])
  },
  methods: {
    ...mapActions(['increment'])
  }

}
</script>
