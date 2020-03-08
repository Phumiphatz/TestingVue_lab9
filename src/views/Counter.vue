<template>
  <div>
    <Mycounter begin="1" @inc="inc" @dec="dec">
      Counter ของฉัน
      <template v-slot:dec>
        ลบ
      </template>
      <template v-slot:inc>
        บวก
      </template>
    </Mycounter>
  </div>
</template>

<script>
import Mycounter from '../components/MyCounter'
export default {
  components: {
    Mycounter
  },
  methods: {
    inc (number) {
      console.log('Counter View inc' + number)
    },
    dec (number) {
      console.log('Counter View dec' + number)
    }
  }
}
</script>

<style></style>
