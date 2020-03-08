<template>
  <div>
    <h1><slot></slot></h1>
    <button @click="dec"><slot name="dec"></slot></button>
    {{ number }}
    <button @click="inc"><slot name="inc"></slot></button>
  </div>
</template>

<script>
export default {
  props: ['begin'],
  data () {
    return {
      number: 0
    }
  },
  methods: {
    dec () {
      this.number--
      this.$emit('dec', this.number)
    },
    inc () {
      this.number++
      this.$emit('inc', this.number)
    }
  }
}
</script>

<style></style>
