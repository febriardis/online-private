<template>
  <div class="header">
    <div class="container-content color-white">
      <a href="javacript:void(0)" class="mr-2" @click="$router.back()">
        <i class="ms-icon icon-arrow_back"></i>
      </a>
      Masuk
    </div>
  </div>
</template>

<script>
export default {
  mounted(){
    console.log('test', this.$router)
  }
}
</script>
