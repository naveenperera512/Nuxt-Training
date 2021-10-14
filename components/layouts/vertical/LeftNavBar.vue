<template>
  <aside class="navbar navbar-vertical navbar-expand-lg navbar-dark">
    <div class="container-fluid">
      <button class="navbar-toggler" data-bs-target="#navbar-menu" data-bs-toggle="collapse" type="button">
        <span class="navbar-toggler-icon"></span>
      </button>
      <h1 class="navbar-brand navbar-brand-autodark">
        <a href=".">
          <img alt="Tabler" class="navbar-brand-image" height="20" src="/" width="110">
        </a>
      </h1>
      <div class="navbar-nav flex-row d-lg-none">
        <div class="nav-item dropdown d-none d-md-flex me-3">
          <a aria-label="Show notifications" class="nav-link px-0" data-bs-toggle="dropdown" href="#" tabindex="-1">
            <!-- Download SVG icon from http://tabler-icons.io/i/bell -->
            <svg class="icon" fill="none" height="24" stroke="currentColor" stroke-linecap="round"
                 stroke-linejoin="round" stroke-width="2" viewBox="0 0 24 24" width="24"
                 xmlns="http://www.w3.org/2000/svg">
              <path d="M0 0h24v24H0z" fill="none" stroke="none"></path>
              <path
                d="M10 5a2 2 0 0 1 4 0a7 7 0 0 1 4 6v3a4 4 0 0 0 2 3h-16a4 4 0 0 0 2 -3v-3a7 7 0 0 1 4 -6"></path>
              <path d="M9 17v1a3 3 0 0 0 6 0v-1"></path>
            </svg>
            <span class="badge bg-red"></span>
          </a>
          <div class="dropdown-menu dropdown-menu-end dropdown-menu-card">
            <div class="card">
              <div class="card-body">
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusamus ad amet consectetur
                exercitationem fugiat in ipsa ipsum, natus odio quidem quod repudiandae sapiente. Amet debitis et
                magni maxime necessitatibus ullam.
              </div>
            </div>
          </div>
        </div>
        <LayoutsVerticalDropdownProfile/>
      </div>
      <!--      side bar-->
      <div id="navbar-menu" class="collapse navbar-collapse">
        <ul class="navbar-nav pt-lg-3">
              <li class="nav-item">
                <nuxt-link :to="{name: 'index'}" class="nav-link">
                  <span class="nav-link-icon d-md-none d-lg-inline-block">
                    <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"></path><polyline points="12 3 20 7.5 20 16.5 12 21 4 16.5 4 7.5 12 3"></polyline><line x1="12" y1="12" x2="20" y2="7.5"></line><line x1="12" y1="12" x2="12" y2="21"></line><line x1="12" y1="12" x2="4" y2="7.5"></line><line x1="16" y1="5.25" x2="8" y2="9.75"></line></svg>
                  </span>
                  <span class="nav-link-title">
                    Interface
                  </span>
              </nuxt-link>
              </li>
              <li class="nav-item dropdown">
                <a class="nav-link dropdown-toggle" href="#navbar-base" data-bs-toggle="dropdown" role="button" aria-expanded="false">
                  <span class="nav-link-icon d-md-none d-lg-inline-block">
                    <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"></path><polyline points="12 3 20 7.5 20 16.5 12 21 4 16.5 4 7.5 12 3"></polyline><line x1="12" y1="12" x2="20" y2="7.5"></line><line x1="12" y1="12" x2="12" y2="21"></line><line x1="12" y1="12" x2="4" y2="7.5"></line><line x1="16" y1="5.25" x2="8" y2="9.75"></line></svg>
                  </span>
                  <span class="nav-link-title">
                    Interface
                  </span>
                </a>
                <div class="dropdown-menu">
                  <div class="dropdown-menu-columns">
                    <div class="dropdown-menu-column">
                      <nuxt-link :to="{name: 'test'}" class="dropdown-item">
                        Sign up
                        </nuxt-link>
                      <a class="dropdown-item" href="./accordion.html">
                        Accordion
                      </a>
                      <a class="dropdown-item" href="./blank.html">
                        Blank page
                      </a>
                    </div>
                  </div>
                </div>
              </li>
            </ul>
      </div>
    </div>

  </aside>
</template>

<script>
  export default {
    
  }
</script>

<style scoped>

</style>
