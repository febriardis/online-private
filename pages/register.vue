<template>
    <div class="register mt-8">
        <div class="container-content mt-6 mb-4">
            <h4 class="color-grey m-0 font-weight-bold">
                Daftar ke Aplikasi
            </h4>
            <h5 class="color-grey font-weight-300 m-0">
                Daftar akun baru untuk masuk ke Aplikasi.
            </h5>
        </div>
        <div class="container-content">
            <div class="tabs-nav">
                <a @click="current_type=1" class="nav-items" :class="{'active':current_type===1}" style="border-radius:10px 0 0 0">Daftar Sebagai Murid</a>
                <a @click="current_type=2" class="nav-items" :class="{'active':current_type===2}" style="border-radius:0 10px 0 0">Daftar Sebagai Pengajar</a>
            </div>
        </div>
        <div class="card pt-4 pb-4" style="min-height: calc(90vh - 10px);">
            <div class="container-content">
                <div class="form-group">
                    <label for="identity" class="color-grey font-weight-300">Nama Lengkap</label>
                    <input type="text" class="form-control" placeholder="Masukan nama lengkap">
                </div>
                <div class="form-group mt-2">
                    <label for="identity" class="color-grey font-weight-300">Email/Nomor Ponsel</label>
                    <input type="text" class="form-control" placeholder="Masukan email atau nomor ponsel">
                </div>
                <div class="form-group mt-2">
                    <label for="identity" class="color-grey font-weight-300">Kata Sandi</label>
                    <input type="text" class="form-control" placeholder="Masukan kata sandi">
                </div>
                <div class="form-group mt-3">
                    <button type="button" class="btn btn-block btn-blue">Daftar</button>
                </div>
                <div class="form-group mt-2 text-center">
                    <span class="font-weight-300 color-grey font-weight-normal">Sudah punya akun?</span> <nuxt-link to="/login" class="color-blue font-weight-300">Klik disini</nuxt-link>
                </div>
                <p class="mt-3 text-center color-grey">Atau</p>
                <div class="form-group mt-2">
                    <button type="button" class="btn btn-block btn-grey">Daftar Dengan Akun Google </button>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        data(){
            return{
                current_type:1
            }
        }
    }
</script>

<style lang="scss">
.tabs-nav{
    display: flex;
    background: #ECECEC;
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
    border-radius: 10px 10px 0px 0px;
    .nav-items{
        padding: 10px;
        flex-basis: 50%;
        text-align: center;
        color: #0AA4E5;
        &.active{
            background: #0AA4E6;
            color: #ffffff;
        }
    }
}
</style>