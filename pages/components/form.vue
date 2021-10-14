<template>
  <div>
    <!--page header-->
    <div class="container-xl">
      <div class="page-header d-print-none">
        <div class="row align-items-center">
          <div class="col">
            <!-- Page pre-title -->
            <h2 class="page-title">
              Add new user
            </h2>
          </div>
          <!-- Page title actions -->
          <div class="col-auto ms-auto d-print-none">
            <!--right-->
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
              <!--card body start-->
              <div class="card-body">
                <!-- Row Start-->
                <div class="row">
                  <div class="col-md-6">
                    <div class="mb-3">
                      <label class="form-label required">First Name</label>
                      <input class="form-control" name="example-password-input" placeholder="Enter first name"
                             type="text">
                    </div>
                  </div>
                  <div class="col-md-6">
                    <div class="mb-3">
                      <label class="form-label required">Last Name</label>
                      <input class="form-control" name="example-password-input" placeholder="Enter last name"
                             type="text">
                    </div>
                  </div>
                </div>
                <!-------------------------- Row End-->
                <!-- Row Start-->
                <div class="row">
                  <div class="col-md-6">
                    <div class="mb-3">
                      <label class="form-label required">Email Address</label>
                      <input class="form-control" name="example-password-input" placeholder="Enter email address"
                             type="email">
                    </div>
                  </div>
                </div>
                <!-------------------------- Row End-->
                <!-- Row Start-->
                <div class="row">
                  <div class="col-md-6">
                    <div class="mb-3">
                      <label class="form-label required">Password</label>
                      <input class="form-control" name="example-password-input" placeholder="Enter password"
                             type="password">
                    </div>
                  </div>
                  <div class="col-md-6">
                    <div class="mb-3">
                      <label class="form-label required">Confirm Password</label>
                      <input class="form-control" name="example-password-input" placeholder="Enter confirm password"
                             type="password">
                    </div>
                  </div>
                </div>
                <!-------------------------- Row End-->
                <!-- Row Start-->
                <div class="row">
                  <div class="col-md-6">
                    <div class="mb-3">
                      <div class="form-label">Gender</div>
                      <div>
                        <label class="form-check form-check-inline">
                          <input class="form-check-input" type="radio" checked="">
                          <span class="form-check-label">Male</span>
                        </label>
                        <label class="form-check form-check-inline">
                          <input class="form-check-input" type="radio">
                          <span class="form-check-label">Female</span>
                        </label>
                      </div>
                    </div>
                  </div>
                </div>
                <!-------------------------- Row End-->
              </div>
              <!---------------------------- card body end-->
              <!--card footer start-->
              <div class="card-footer text-end">
                <div class="d-flex">
                  <a class="btn btn-link" href="#">Cancel</a>
                  <button class="btn btn-primary ms-auto" type="submit">Create user</button>
                </div>
              </div>
              <!----------------------------card footer end-->
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

  }
</script>

<style scoped>

</style>
