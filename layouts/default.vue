<template>
  <div class="container-center">
    <!-- header -->
    <Header />
    <!-- /header -->
    <router-view />
  </div>
</template>

<script>
import Header from './components/header'
export default {
  components: {
    Header
  }
}
</script>

<style>
@import url('../styles/app.scss');
</style>
