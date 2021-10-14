<template>
  <div :class="[sticky? 'sticky-top': '']">
    <!--    header-->
    <header class="navbar navbar-expand-md navbar-light d-print-none">
      <div class="container-xl">
        <button
          class="navbar-toggler"
          data-bs-target="#navbar-menu"
          data-bs-toggle="collapse"
          type="button"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <h1
          class="navbar-brand navbar-brand-autodark d-none-navbar-horizontal pe-0 pe-md-3"
        >
          <a href=".">
            <img
              alt="Tabler"
              class="navbar-brand-image"
              style="height: 1.6rem; width: 7rem"
              height="35"
              src="/logo.png"
              width="150"
            />
          </a>
        </h1>
        <div class="navbar-nav flex-row order-md-last">
          <div class="nav-item d-none d-md-flex me-3">
            <div class="btn-list">
              <a
                class="btn btn-outline-white"
                href="https://github.com/tabler/tabler"
                rel="noreferrer"
                target="_blank"
              >
                <!-- Download SVG icon from http://tabler-icons.io/i/brand-github -->
                <svg
                  class="icon text-github"
                  fill="none"
                  height="24"
                  stroke="currentColor"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  viewBox="0 0 24 24"
                  width="24"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path d="M0 0h24v24H0z" fill="none" stroke="none"/>
                  <path
                    d="M9 19c-4.3 1.4 -4.3 -2.5 -6 -3m12 5v-3.5c0 -1 .1 -1.4 -.5 -2c2.8 -.3 5.5 -1.4 5.5 -6a4.6 4.6 0 0 0 -1.3 -3.2a4.2 4.2 0 0 0 -.1 -3.2s-1.1 -.3 -3.5 1.3a12.3 12.3 0 0 0 -6.2 0c-2.4 -1.6 -3.5 -1.3 -3.5 -1.3a4.2 4.2 0 0 0 -.1 3.2a4.6 4.6 0 0 0 -1.3 3.2c0 4.6 2.7 5.7 5.5 6c-.6 .6 -.6 1.2 -.5 2v3.5"
                  />
                </svg>
                Source code
              </a>
              <a
                class="btn btn-outline-white"
                href="https://github.com/sponsors/codecalm"
                rel="noreferrer"
                target="_blank"
              >
                <!-- Download SVG icon from http://tabler-icons.io/i/heart -->
                <svg
                  class="icon text-pink"
                  fill="none"
                  height="24"
                  stroke="currentColor"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  viewBox="0 0 24 24"
                  width="24"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path d="M0 0h24v24H0z" fill="none" stroke="none"/>
                  <path
                    d="M19.5 13.572l-7.5 7.428l-7.5 -7.428m0 0a5 5 0 1 1 7.5 -6.566a5 5 0 1 1 7.5 6.572"
                  />
                </svg>
                Sponsor
              </a>
            </div>
          </div>
          <div class="nav-item dropdown d-none d-md-flex me-3">
            <a
              aria-label="Show notifications"
              class="nav-link px-0"
              data-bs-toggle="dropdown"
              href="#"
              tabindex="-1"
            >
              <!-- Download SVG icon from http://tabler-icons.io/i/bell -->
              <svg
                class="icon"
                fill="none"
                height="24"
                stroke="currentColor"
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                viewBox="0 0 24 24"
                width="24"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path d="M0 0h24v24H0z" fill="none" stroke="none"/>
                <path
                  d="M10 5a2 2 0 0 1 4 0a7 7 0 0 1 4 6v3a4 4 0 0 0 2 3h-16a4 4 0 0 0 2 -3v-3a7 7 0 0 1 4 -6"
                />
                <path d="M9 17v1a3 3 0 0 0 6 0v-1"/>
              </svg>
              <span class="badge bg-red"></span>
            </a>
            <div class="dropdown-menu dropdown-menu-end dropdown-menu-card">
              <div class="card">
                <div class="card-body">
                  Lorem ipsum dolor sit amet, consectetur adipisicing elit.
                  Accusamus ad amet consectetur exercitationem fugiat in ipsa
                  ipsum, natus odio quidem quod repudiandae sapiente. Amet
                  debitis et magni maxime necessitatibus ullam.
                </div>
              </div>
            </div>
          </div>
          <div class="nav-item dropdown">
            <a
              aria-label="Open user menu"
              class="nav-link d-flex lh-1 text-reset p-0"
              data-bs-toggle="dropdown"
              href="#"
            >
              <span
                class="avatar avatar-sm"
                style="background-image: url(https://data.whicdn.com/images/322027365/original.jpg?t=1541703413)"
              ></span>
              <div class="d-none d-xl-block ps-2">
                <div>Paweł Kuna</div>
                <div class="mt-1 small text-muted">UI Designer</div>
              </div>
            </a>
            <div class="dropdown-menu dropdown-menu-end dropdown-menu-arrow">
              <a class="dropdown-item" href="#">Set status</a>
              <a class="dropdown-item" href="#">Profile & account</a>
              <a class="dropdown-item" href="#">Feedback</a>
              <div class="dropdown-divider"></div>
              <a class="dropdown-item" href="#">Settings</a>
              <a class="dropdown-item" href="#">Logout</a>
            </div>
          </div>
        </div>
      </div>
    </header>

    <!--    navBar-->
    


  </div>





</template>

<script>
  export default {
    data() {
      return {
        sticky: true,
        navBarRoutes: [
          {
            name: "Home",
            path: "/index",
            icon: "<svg xmlns=\"http://www.w3.org/2000/svg\" class=\"icon icon-tabler icon-tabler-home\" width=\"24\" height=\"24\" viewBox=\"0 0 24 24\" stroke-width=\"2\" stroke=\"currentColor\" fill=\"none\" stroke-linecap=\"round\" stroke-linejoin=\"round\">\n" +
              "   <path stroke=\"none\" d=\"M0 0h24v24H0z\" fill=\"none\"></path>\n" +
              "   <polyline points=\"5 12 3 12 12 3 21 12 19 12\"></polyline>\n" +
              "   <path d=\"M5 12v7a2 2 0 0 0 2 2h10a2 2 0 0 0 2 -2v-7\"></path>\n" +
              "   <path d=\"M9 21v-6a2 2 0 0 1 2 -2h2a2 2 0 0 1 2 2v6\"></path>\n" +
              "</svg>"
          },
          {
            name: "Sub Links",
            path: "/index",
            icon: "<svg xmlns=\"http://www.w3.org/2000/svg\" class=\"icon icon-tabler icon-tabler-layers-subtract\" width=\"24\" height=\"24\" viewBox=\"0 0 24 24\" stroke-width=\"2\" stroke=\"currentColor\" fill=\"none\" stroke-linecap=\"round\" stroke-linejoin=\"round\">\n" +
              "   <path stroke=\"none\" d=\"M0 0h24v24H0z\" fill=\"none\"></path>\n" +
              "   <rect x=\"8\" y=\"4\" width=\"12\" height=\"12\" rx=\"2\"></rect>\n" +
              "   <path d=\"M16 16v2a2 2 0 0 1 -2 2h-8a2 2 0 0 1 -2 -2v-8a2 2 0 0 1 2 -2h2\"></path>\n" +
              "</svg>",
            children: [
              [
                {
                  name: "Sub 1",
                  path: "/index",
                },
                {
                  name: "Sub 2",
                  path: "/index",
                },
              ],
              [
                {
                  name: "Sub 1",
                  path: "/index",
                },
                {
                  name: "Sub 2",
                  path: "/index",
                },
              ]
            ]
          },
        ]
      }
    }
  };
</script>

<style lang="scss" scoped></style>
