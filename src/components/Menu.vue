<template>
  <div>
    <b-nav>
      <b-nav-item active><router-link to="/">Home</router-link></b-nav-item>
      <b-nav-item
        ><router-link to="/showview">Showview</router-link></b-nav-item
      >
      <b-nav-item><router-link to="/form">Form</router-link></b-nav-item>
      <b-nav-item><router-link to="/table">Table</router-link></b-nav-item>

      <b-nav-item><router-link to="/about">About</router-link></b-nav-item>
      <b-nav-item><router-link to="/counter">Counter</router-link></b-nav-item>
    </b-nav>
  </div>
</template>

<script>
export default {}
</script>

<style></style>
