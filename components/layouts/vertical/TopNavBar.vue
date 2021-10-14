<template>
  <header class="navbar navbar-expand-md navbar-light d-none d-lg-flex d-print-none">
    <div class="container-xl">
      <button class="navbar-toggler" data-bs-target="#navbar-menu" data-bs-toggle="collapse" type="button">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="navbar-nav flex-row order-md-last">
        <div class="nav-item dropdown d-none d-md-flex me-3">
          <a aria-label="Show notifications" class="nav-link px-0" data-bs-toggle="dropdown" href="#" tabindex="-1">
            <!-- Download SVG icon from http://tabler-icons.io/i/bell -->
            <svg class="icon" fill="none" height="24" stroke="currentColor" stroke-linecap="round"
                 stroke-linejoin="round" stroke-width="2" viewBox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg">
              <path d="M0 0h24v24H0z" fill="none" stroke="none"></path>
              <path d="M10 5a2 2 0 0 1 4 0a7 7 0 0 1 4 6v3a4 4 0 0 0 2 3h-16a4 4 0 0 0 2 -3v-3a7 7 0 0 1 4 -6"></path>
              <path d="M9 17v1a3 3 0 0 0 6 0v-1"></path>
            </svg>
            <span class="badge bg-red"></span>
          </a>
          <div class="dropdown-menu dropdown-menu-end dropdown-menu-card">
            <div class="card">
              <div class="card-body">
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusamus ad amet consectetur exercitationem
                fugiat in ipsa ipsum, natus odio quidem quod repudiandae sapiente. Amet debitis et magni maxime
                necessitatibus ullam.
              </div>
            </div>
          </div>
        </div>
        <LayoutsVerticalDropdownProfile/>
      </div>
      <div id="navbar-menu" class="collapse navbar-collapse">
        <div>
          <form action="." method="get">
            <div class="input-icon">
                  <span class="input-icon-addon">
                    <!-- Download SVG icon from http://tabler-icons.io/i/search -->
                    <svg class="icon" fill="none" height="24" stroke="currentColor" stroke-linecap="round"
                         stroke-linejoin="round" stroke-width="2" viewBox="0 0 24 24" width="24"
                         xmlns="http://www.w3.org/2000/svg"><path d="M0 0h24v24H0z" fill="none" stroke="none"></path><circle
                      cx="10" cy="10" r="7"></circle><line x1="21" x2="15" y1="21" y2="15"></line></svg>
                  </span>
              <input aria-label="Search in website" class="form-control" placeholder="Search…" type="text">
            </div>
          </form>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
  export default {
  }
</script>

<style scoped>

</style>
