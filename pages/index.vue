<template>
  <div>
    <div class="container-xl">
      <!-- Page title -->
      <div class="page-header d-print-none">
        <div class="row align-items-center">
          <div class="col">
            <h2 class="page-title">
              Home
            </h2>
          </div>
        </div>
      </div>
    </div>
    <div class="page-body">
      <div class="container-xl">
          <div class="card">
            <div class="card-body">
              <!-- Page title -->
                <div class="row align-items-center">
                  <div class="col">
                    <h2 class="page-title">
                      Dashboard
                    </h2>
                  </div>
                  <!-- Page title actions -->
                  <div class="col-auto ms-auto d-print-none">
                    <div class="btn-list">
                  <span class="d-none d-sm-inline">
                    <a href="#" class="btn btn-white">
                      New view
                    </a>
                  </span>
                      <a href="#" class="btn btn-primary d-none d-sm-inline-block" data-bs-toggle="modal" data-bs-target="#modal-report">
                        <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"></path><line x1="12" y1="5" x2="12" y2="19"></line><line x1="5" y1="12" x2="19" y2="12"></line></svg>
                        Create new report
                      </a>
                    </div>
                  </div>
                </div>
            </div>
            <div class="table-responsive">
              <div class="card-body border-bottom py-3">
                <div class="d-flex">
                  <div class="text-muted">
                    Show
                    <div class="mx-2 d-inline-block">
                      <input type="text" class="form-control form-control-sm" value="8" size="3" aria-label="Invoices count">
                    </div>
                    entries
                  </div>
                  <div class="ms-auto text-muted">
                    Search:
                    <div class="ms-2 d-inline-block">
                      <input type="text" class="form-control form-control-sm" aria-label="Search invoice">
                    </div>
                  </div>
                </div>
              </div>
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
                <tr>
                  <td data-label="Name">
                    <div class="d-flex py-1 align-items-center">
                      <span class="avatar me-2">TK</span>
                      <div class="flex-fill">
                        <div class="font-weight-medium">Thatcher Keel</div>
                        <div class="text-muted"><a href="#" class="text-reset">tkeelf@blogger.com</a></div>
                      </div>
                    </div>
                  </td>
                  <td data-label="Title">
                    <div>VP Sales</div>
                    <div class="text-muted">Business Development</div>
                  </td>
                  <td class="text-muted" data-label="Role">
                    User
                  </td>
                  <td>
                    <div class="btn-list flex-nowrap">
                      <a href="#" class="btn btn-white">
                        Edit
                      </a>
                      <div class="dropdown">
                        <button class="btn dropdown-toggle align-text-top" data-bs-boundary="viewport" data-bs-toggle="dropdown">
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
                <tr>
                  <td data-label="Name">
                    <div class="d-flex py-1 align-items-center">
                      <span class="avatar me-2">DE</span>
                      <div class="flex-fill">
                        <div class="font-weight-medium">Dyann Escala</div>
                        <div class="text-muted"><a href="#" class="text-reset">descalag@usatoday.com</a></div>
                      </div>
                    </div>
                  </td>
                  <td data-label="Title">
                    <div>Mechanical Systems Engineer</div>
                    <div class="text-muted">Sales</div>
                  </td>
                  <td class="text-muted" data-label="Role">
                    Admin
                  </td>
                  <td>
                    <div class="btn-list flex-nowrap">
                      <a href="#" class="btn btn-white">
                        Edit
                      </a>
                      <div class="dropdown">
                        <button class="btn dropdown-toggle align-text-top" data-bs-boundary="viewport" data-bs-toggle="dropdown">
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
                <tr>
                  <td data-label="Name">
                    <div class="d-flex py-1 align-items-center">
                      <span class="avatar me-2">AM</span>
                      <div class="flex-fill">
                        <div class="font-weight-medium">Avivah Mugleston</div>
                        <div class="text-muted"><a href="#" class="text-reset">amuglestonh@intel.com</a></div>
                      </div>
                    </div>
                  </td>
                  <td data-label="Title">
                    <div>Actuary</div>
                    <div class="text-muted">Sales</div>
                  </td>
                  <td class="text-muted" data-label="Role">
                    User
                  </td>
                  <td>
                    <div class="btn-list flex-nowrap">
                      <a href="#" class="btn btn-white">
                        Edit
                      </a>
                      <div class="dropdown">
                        <button class="btn dropdown-toggle align-text-top" data-bs-boundary="viewport" data-bs-toggle="dropdown">
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
                <tr>
                  <td data-label="Name">
                    <div class="d-flex py-1 align-items-center">
                      <span class="avatar me-2">AA</span>
                      <div class="flex-fill">
                        <div class="font-weight-medium">Arlie Armstead</div>
                        <div class="text-muted"><a href="#" class="text-reset">aarmsteadi@yellowpages.com</a></div>
                      </div>
                    </div>
                  </td>
                  <td data-label="Title">
                    <div>VP Quality Control</div>
                    <div class="text-muted">Accounting</div>
                  </td>
                  <td class="text-muted" data-label="Role">
                    Owner
                  </td>
                  <td>
                    <div class="btn-list flex-nowrap">
                      <a href="#" class="btn btn-white">
                        Edit
                      </a>
                      <div class="dropdown">
                        <button class="btn dropdown-toggle align-text-top" data-bs-boundary="viewport" data-bs-toggle="dropdown">
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
                <tr>
                  <td data-label="Name">
                    <div class="d-flex py-1 align-items-center">
                      <span class="avatar me-2">TC</span>
                      <div class="flex-fill">
                        <div class="font-weight-medium">Tessie Curzon</div>
                        <div class="text-muted"><a href="#" class="text-reset">tcurzonj@hp.com</a></div>
                      </div>
                    </div>
                  </td>
                  <td data-label="Title">
                    <div>Research Nurse</div>
                    <div class="text-muted">Product Management</div>
                  </td>
                  <td class="text-muted" data-label="Role">
                    Admin
                  </td>
                  <td>
                    <div class="btn-list flex-nowrap">
                      <a href="#" class="btn btn-white">
                        Edit
                      </a>
                      <div class="dropdown">
                        <button class="btn dropdown-toggle align-text-top" data-bs-boundary="viewport" data-bs-toggle="dropdown" aria-expanded="false">
                          Actions
                        </button>
                        <div class="dropdown-menu dropdown-menu-end" style="">
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
            <div class="card-footer d-flex align-items-center">
              <p class="m-0 text-muted">Showing <span>1</span> to <span>8</span> of <span>16</span> entries</p>
              <ul class="pagination m-0 ms-auto">
                <li class="page-item disabled">
                  <a class="page-link" href="#" tabindex="-1" aria-disabled="true">
                    <!-- Download SVG icon from http://tabler-icons.io/i/chevron-left -->
                    <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"></path><polyline points="15 6 9 12 15 18"></polyline></svg>
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
                    <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"></path><polyline points="9 6 15 12 9 18"></polyline></svg>
                  </a>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>
</template>

<script>
export default {
  layout: "vertical"
};
</script>
