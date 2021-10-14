<template>
  <div class="antialiased border-top-wide border-primary d-flex flex-column" data-gr-ext-installed=""
       data-new-gr-c-s-check-loaded="14.1032.0">
    <div class="page page-center">
      <div class="container-tight py-4">
        <!-- <div class="text-center mb-4">
          <a href="."><img alt="" height="36" src="/logo.png"></a>
        </div> -->
        <form autocomplete="off" class="card card-md" @submit.prevent="login">
          <div class="card-body">
            <h2 class="card-title text-center mb-4">Login to your account</h2>

            <div class="mb-3">
              <label class="form-label ">Email address</label>
              <input v-model="form.email" class="form-control " placeholder="Enter email"
                     type="email" :class="[errors.email ? 'is-invalid': '']">
              <div v-if="errors.email" class="invalid-feedback">{{errors.email[0]}}</div>
            </div>

            <div class="mb-2">
              <label class="form-label">
                Password
                <span class="form-label-description">
                  <nuxt-link :to="{name: 'auth-reset_password-forgot-password'}">I forgot password</nuxt-link>
                </span>
              </label>
              <div class="input-group input-group-flat">
                <input v-model="form.password" :type="password_type" autocomplete="off" class="form-control"
                       placeholder="Password" :class="[errors.password ? 'is-invalid': '']">
                <div v-if="errors.password" class="invalid-feedback">{{errors.password[0]}}</div>
                <span class="input-group-text" @click.prevent="passwordToggle">
                  <a v-if="password_type==='password'" class="link-secondary" data-bs-original-title="Show password" data-bs-toggle="tooltip"
                     href="#" title="">
                    <svg class="icon" fill="none" height="24" stroke="currentColor" stroke-linecap="round"
                         stroke-linejoin="round" stroke-width="2" viewBox="0 0 24 24" width="24"
                         xmlns="http://www.w3.org/2000/svg"><path d="M0 0h24v24H0z" fill="none" stroke="none"></path><circle
                      cx="12" cy="12" r="2"></circle><path
                      d="M22 12c-2.667 4.667 -6 7 -10 7s-7.333 -2.333 -10 -7c2.667 -4.667 6 -7 10 -7s7.333 2.333 10 7"></path></svg>

                  </a>
                   <a v-else class="link-secondary" data-bs-original-title="Show password" data-bs-toggle="tooltip"
                      href="#" title="">
                   <svg class="icon icon-tabler icon-tabler-eye-off" fill="none" height="24"
                        stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                        viewBox="0 0 24 24"
                        width="24" xmlns="http://www.w3.org/2000/svg">
                       <path d="M0 0h24v24H0z" fill="none" stroke="none"></path>
                       <line x1="3" x2="21" y1="3" y2="21"></line>
                       <path d="M10.584 10.587a2 2 0 0 0 2.828 2.83"></path>
                       <path
                         d="M9.363 5.365a9.466 9.466 0 0 1 2.637 -.365c4 0 7.333 2.333 10 7c-.778 1.361 -1.612 2.524 -2.503 3.488m-2.14 1.861c-1.631 1.1 -3.415 1.651 -5.357 1.651c-4 0 -7.333 -2.333 -10 -7c1.369 -2.395 2.913 -4.175 4.632 -5.341"></path>
                    </svg>
                  </a>
                </span>
              </div>
            </div>
            <div class="mb-2">
              <label class="form-check">
                <input v-model="form.remember_me" class="form-check-input" type="checkbox">
                <span class="form-check-label">Remember me on this device</span>
              </label>
            </div>
            <div class="form-footer">
              <button class="btn btn-primary w-100" type="submit">Sign in</button>
            </div>
          </div>
        </form>
        <div class="text-center text-muted mt-3">
          Don't have account yet? <nuxt-link :to="{name: 'auth-register'}">Sign up</nuxt-link>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    auth: 'guest',
    data() {
      return {
        form: {
          email: "",
          password: "",
          remember_me: ""
        },
        errors: [],
        password_type: 'password'
      }
    },
    methods: {
      async login() {
        try {
          await this.$auth.loginWith('laravelSanctum', {data: this.form});
        } catch (e) {
          if (e.response.status === 422) this.errors = e.response.data.errors;
        }
      },
      passwordToggle() {
        this.password_type = (this.password_type === "password") ? 'text' : 'password';
      }
    }
  }
</script>

<style scoped>

</style>
