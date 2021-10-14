<template>
<div class="row justify-content-center">
    <div class="col-md-6 col-lg-6 col-xl-5">
        <div class="card mt-5">
            <div class="card-body p-4">
                <div class="text-center w-75 m-auto">
                    <p class="text-muted mb-4 mt-3">Don't have an account? Create your own account.</p>
                </div>

                <form action="#">
                    <div class="form-group mb-3">
                        <label for="name">Full Name</label>
                        <input id="name" class="form-control" type="text" required placeholder="Enter your name" />
                    </div>

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
                        <label for="password_confirmation">Password Confirmation</label>
                        <div class="input-group input-group-merge">
                            <input id="password_confirmation" type="password" class="form-control" placeholder="Enter your password confirmation" />
                            <div class="input-group-append" data-password_confirmation="false">
                                <div class="input-group-text">
                                    <i class="fa fa-eye-slash" aria-hidden="true"></i>
                                </div>
                            </div>
                        </div>
                    </div>

                    <div class="form-group mb-0 text-center">
                        <button class="btn btn-primary btn-block" type="submit">Sign Up</button>
                    </div>
                </form>
            </div>
            <!-- end card-body -->
        </div>
        <!-- end card -->

        <div class="row mt-3">
            <div class="col-12 text-center">
                <p class="text-muted">
                    Already have account?
                    <nuxt-link to="/auth/login" class="text-primary font-weight-medium ml-1">Sign In</nuxt-link>
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