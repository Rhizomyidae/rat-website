<template>
  <div class="hello">
    <!-- Preloader -->
    <div class="preloader" v-if="preloader">
      <div class="spinner-border text-primary" role="status">
        <span class="sr-only">Loading...</span>
      </div>
    </div>
    <div class="modal fade" tabindex="-1" role="dialog" id="modal-cookies" data-backdrop="false" aria-labelledby="modal-cookies" aria-hidden="true">
      <div class="modal-dialog modal-dialog-aside left-4 right-4 bottom-4">
        <div class="modal-content bg-dark-dark">
          <div class="modal-body">
            <!-- Text -->
            <p class="text-sm text-white mb-3">
              We use cookies so that our themes work for you. By using our website, you agree to our use of cookies.
            </p>
            <!-- Buttons -->
            <a href="pages/utility/terms.html" class="btn btn-sm btn-white" target="_blank">Learn more</a>
            <button type="button" class="btn btn-sm btn-primary mr-2" data-dismiss="modal">OK</button>
          </div>
        </div>
      </div>
    </div>
    <!-- Navbar -->
    <nav class="navbar navbar-expand-lg navbar-light bg-white">
      <div class="container">
        <!-- Brand -->
        <a class="navbar-brand" href="index.html">
          <img alt="Image placeholder" src="http://qb1t0tazy.bkt.clouddn.com/assets/img/brand/dark.svg" id="navbar-logo">
        </a>
        <!-- Toggler -->
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarCollapse" aria-controls="navbarCollapse" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <!-- Collapse -->
        <div class="collapse navbar-collapse" id="navbarCollapse">
          <ul class="navbar-nav mt-4 mt-lg-0 ml-auto">
            <li class="nav-item ">
              <a class="nav-link" href="/overview">Overview</a>
            </li>
            <li class="nav-item dropdown dropdown-animate" data-toggle="hover">
              <a class="nav-link" href="#" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">Pages</a>
              <div class="dropdown-menu dropdown-menu-single">
                <a href="/" class="dropdown-item">Homepage</a>
                <a href="/about" class="dropdown-item">About us</a>
                <a href="/contact" class="dropdown-item">Contact</a>
                <div class="dropdown-divider"></div>
<!--                <a href="login.html" class="dropdown-item">Login</a>-->
              </div>
            </li>
            <li class="nav-item ">
              <a class="nav-link" href="/docs">Docs</a>
            </li>
          </ul>
          <!-- Button -->
<!--          <a class="navbar-btn btn btn-sm btn-primary d-none d-lg-inline-block ml-3" href="">-->
<!--            Download Free-->
<!--          </a>-->
          <!-- Mobile button -->
          <div class="d-lg-none text-center">
            <a href="#" class="btn btn-block btn-sm btn-warning">See more details</a>
          </div>
        </div>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  name: "Header",
  props: {
    msg: String
  },
  data: function() {
    return {
      preloader: false
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
