<template>
  <b-container fluid>
    <b-row>
      <b-col> <Header /> </b-col>
    </b-row>
    <b-row>
      <b-col cols="2"> <Menu /> </b-col>
      <b-col> <router-view></router-view> </b-col>
    </b-row>
  </b-container>
</template>

<script>
import Header from './Header'
import Menu from './Menu'
export default {
  components: {
    Header,
    Menu
  }
}
</script>

<style></style>
