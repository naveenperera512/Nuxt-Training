<template>
  <div>

    <!--    page header-->
    <div class="container-xl">
      <div class="page-header d-print-none">
        <div class="row align-items-center">
          <div class="col">
            <!-- Page pre-title -->
            <div class="page-pretitle">
              Overview
            </div>
            <h2 class="page-title">
              Dashboard
            </h2>
          </div>
          <!-- Page title actions -->
          <div class="col-auto ms-auto d-print-none">
            <div class="btn-list">
              <a class="btn btn-primary d-none d-sm-inline-block" data-bs-target="#modal-report" data-bs-toggle="modal"
                 href="#">
                <!-- Download SVG icon from http://tabler-icons.io/i/plus -->
                <svg class="icon" fill="none" height="24" stroke="currentColor" stroke-linecap="round"
                     stroke-linejoin="round" stroke-width="2" viewBox="0 0 24 24" width="24"
                     xmlns="http://www.w3.org/2000/svg">
                  <path d="M0 0h24v24H0z" fill="none" stroke="none"></path>
                  <line x1="12" x2="12" y1="5" y2="19"></line>
                  <line x1="5" x2="19" y1="12" y2="12"></line>
                </svg>
                Create new [............]
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!--    page body-->
    <div class="page-body">
      <div class="container-xl">
        <div class="row row-cards">
          <div class="col-12">
            <div class="card">
              <!--table-->
              <div class="table-responsive">
                <table class="table table-vcenter table-mobile-md card-table">
                  <thead>
                  <tr>
                    <th>Name</th>
                    <th>Title</th>
                    <th>Role</th>
                    <th class="w-1"></th>
                  </tr>
                  </thead>
                  <tbody>
                  <tr v-for="user in users">
                    <td  data-label="Name">
                      <div class="d-flex py-1 align-items-center">
                        <span class="avatar me-2" style="background-image: url(./static/avatars/010m.jpg)"></span>
                        <div class="flex-fill">
                          <div class="font-weight-medium">{{user.name}}</div>
                          <div class="text-muted"><a class="text-reset" href="#">{{user.email}}</a></div>
                        </div>
                      </div>
                    </td>
                    <td data-label="Title">
                      <div>{{user.title}}</div>
                      <div class="text-muted">{{user.department}}</div>
                    </td>
                    <td class="text-muted" data-label="Role">
                      {{user.role}}
                    </td>
                    <td>
                      <div class="btn-list flex-nowrap">
                        <a class="btn btn-white" href="#">
                          Edit
                        </a>
                        <div class="dropdown">
                          <button class="btn dropdown-toggle align-text-top" data-bs-boundary="viewport"
                                  data-bs-toggle="dropdown">
                            Actions
                          </button>
                          <div class="dropdown-menu dropdown-menu-end">
                            <a class="dropdown-item" href="#">
                              Action
                            </a>
                            <a class="dropdown-item" href="#">
                              Another action
                            </a>
                          </div>
                        </div>
                      </div>
                    </td>
                  </tr>
                  </tbody>
                </table>
              </div>
              <!--pagination-->
              <ul class="pagination justify-content-center justify-content-md-end ">
                <li class="page-item disabled">
                  <a aria-disabled="true" class="page-link" href="#" tabindex="-1">
                    <!-- Download SVG icon from http://tabler-icons.io/i/chevron-left -->
                    <svg class="icon" fill="none" height="24" stroke="currentColor" stroke-linecap="round"
                         stroke-linejoin="round" stroke-width="2" viewBox="0 0 24 24" width="24"
                         xmlns="http://www.w3.org/2000/svg">
                      <path d="M0 0h24v24H0z" fill="none" stroke="none"></path>
                      <polyline points="15 6 9 12 15 18"></polyline>
                    </svg>
                    prev
                  </a>
                </li>
                <li class="page-item"><a class="page-link" href="#">1</a></li>
                <li class="page-item active"><a class="page-link" href="#">2</a></li>
                <li class="page-item"><a class="page-link" href="#">3</a></li>
                <li class="page-item"><a class="page-link" href="#">4</a></li>
                <li class="page-item"><a class="page-link" href="#">5</a></li>
                <li class="page-item">
                  <a class="page-link" href="#">
                    next <!-- Download SVG icon from http://tabler-icons.io/i/chevron-right -->
                    <svg class="icon" fill="none" height="24" stroke="currentColor" stroke-linecap="round"
                         stroke-linejoin="round" stroke-width="2" viewBox="0 0 24 24" width="24"
                         xmlns="http://www.w3.org/2000/svg">
                      <path d="M0 0h24v24H0z" fill="none" stroke="none"></path>
                      <polyline points="9 6 15 12 9 18"></polyline>
                    </svg>
                  </a>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>

  </div>
</template>

<script>
  export default {
    layout: "horizontal",
    data () {
      return {
        users: [
          {
            name: "Thatcher Keel",
            email: "tkeelf@blogger.com",
            title: "VP Sales",
            department: "Business Development",
            role: "User"
          },
          {
            name: "Dyann Escala",
            email: "descalag@usatoday.com",
            title: "Mechanical Systems Engineer\n",
            department: "Sales",
            role: "Admin"
          },
          {
            name: "Avivah Mugleston",
            email: "amuglestonh@intel.com",
            title: "Actuary\n",
            department: "Sales",
            role: "User"
          },
          {
            name: "Arlie Armstead",
            email: "aarmsteadi@yellowpages.com",
            title: "VP Quality Control",
            department: "Accounting",
            role: "Owner"
          },
          {
            name: "Tessie Curzon",
            email: "tcurzonj@hp.com",
            title: "Research Nurse",
            department: "Product Management",
            role: "Admin"
          },
        ]
      }
    }
  }
</script>

<style scoped>

</style>
