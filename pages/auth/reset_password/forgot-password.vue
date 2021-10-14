<template>
<div class="row justify-content-center">
    <div class="col-md-6 col-lg-6 col-xl-5">
        <div class="card mt-5">
            <div class="card-body p-4">
                <div class="text-center w-75 m-auto">
                    <p class="text-muted mb-4 mt-3">Enter your email address and password to access admin panel.</p>
                </div>

                <form action="#">
                    <div class="form-group mb-3">
                        <label for="emailaddress">Email address</label>
                        <input id="emailaddress" class="form-control" type="email" required placeholder="Enter your email" />
                    </div>

                    <div class="form-group mb-3">
                        <label for="password">Password</label>
                        <div class="input-group input-group-merge">
                            <input id="password" type="password" class="form-control" placeholder="Enter your password" />
                            <div class="input-group-append" data-password="false">
                                <div class="input-group-text">
                                    <i class="fa fa-eye-slash" aria-hidden="true"></i>
                                </div>
                            </div>
                        </div>
                    </div>

                    <div class="form-group mb-3">
                        <div class="custom-control custom-checkbox">
                            <input id="checkbox-signin" type="checkbox" class="custom-control-input" checked />
                            <label class="custom-control-label" for="checkbox-signin">Remember me</label>
                        </div>
                    </div>

                    <div class="form-group mb-0 text-center">
                        <button class="btn btn-primary btn-block" type="submit">Log In</button>
                    </div>
                </form>
            </div>
            <!-- end card-body -->
        </div>
        <!-- end card -->

        <div class="row mt-3">
            <div class="col-12 text-center">
                <p>
                    <nuxt-link to="/auth/recoverpwd" class="text-muted ml-1">Forgot your password?</nuxt-link>
                </p>
                <p class="text-muted">
                    Don't have an account?
                    <nuxt-link to="/auth/register" class="text-primary font-weight-medium ml-1">Sign Up</nuxt-link>
                </p>
            </div>
            <!-- end col -->
        </div>
        <!-- end row -->
    </div>
    <!-- end col -->
</div>
<!-- end row -->
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>

</style>