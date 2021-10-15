<template>
  <div class="nav-item dropdown">
    <a aria-label="Open user menu" class="nav-link d-flex lh-1 text-reset p-0" data-bs-toggle="dropdown" href="#">
      <span class="avatar avatar-sm" style="background-image: url(./static/avatars/000m.jpg)">SA</span>
      <div class="d-none d-xl-block ps-2">
        <div>{{$auth.user.name}}</div>
        <div class="mt-1 small text-muted">Online</div>
      </div>
    </a>
    <div class="dropdown-menu dropdown-menu-end dropdown-menu-arrow">
      <nuxt-link :to="{name: 'profile'}" class="dropdown-item">Profile &amp; account</nuxt-link>
      <a class="dropdown-item" href="#" @click.prevent="logout">Logout</a>
    </div>
  </div>
</template>

<script>
  export default {
    methods: {
      async logout() {
        await this.$auth.logout();
        this.$router.replace({name: 'auth-login'});
      }
    }
  }
</script>

<style scoped>

</style>
