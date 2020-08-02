<template>
  <div class="login mt-8">
    <div class="container-content mb-4">
      <h4 class="color-grey m-0 font-weight-bold">
        Masuk ke Aplikasi
      </h4>
      <h5 class="color-grey font-weight-300 m-0">
        Masuk dengan akun yang telah dibuat.
      </h5>
    </div>
    <div class="card pt-4 pb-4" style="min-height: calc(100vh - 60px);">
      <div class="container-content">
        <div class="form-group">
          <label for="identity" class="color-grey font-weight-300">Email/Nomor Ponsel</label>
          <input type="text" class="form-control" placeholder="Masukan email atau nomor ponsel">
        </div>
        <div class="form-group mt-2">
          <label for="identity" class="color-grey font-weight-300">Kata Sandi</label>
          <input type="text" class="form-control" placeholder="Masukan kata sandi">
        </div>
        <div class="form-group mt-2">
          <a href="#" class="color-blue font-weight-300">Password lupa?</a>
        </div>
        <div class="form-group mt-2">
          <button type="button" class="btn btn-block btn-blue">Masuk</button>
        </div>
        <div class="form-group mt-2 text-center">
          <span class="font-weight-300 color-grey font-weight-normal">Belum punya akun?</span> <nuxt-link to="/register" class="color-blue font-weight-300">Klik disini</nuxt-link>
        </div>
        <p class="mt-3 text-center color-grey">
          Atau
        </p>
        <div class="form-group mt-2">
          <button type="button" class="btn btn-block btn-grey">Masuk Dengan Akun Google </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>
