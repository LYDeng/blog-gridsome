<!--
 * @Date: 2021-10-11 09:38:09
 * @LastEditors: lyd
 * @LastEditTime: 2021-10-12 17:22:38
 * @Description: 无
-->
<template>
  <div class="layout">
    <!-- Navigation -->
    <nav class="navbar navbar-expand-lg navbar-light fixed-top" id="mainNav">
      <div class="container">
        <g-link class="navbar-brand" to="/">HOME</g-link>
        <button class="navbar-toggler navbar-toggler-right" type="button" data-toggle="collapse" data-target="#navbarResponsive" aria-controls="navbarResponsive" aria-expanded="false" aria-label="Toggle navigation">
          Menu
          <i class="fas fa-bars"></i>
        </button>
        <div class="collapse navbar-collapse" id="navbarResponsive">
          <ul class="navbar-nav ml-auto">
            <li class="nav-item">
              <g-link to="/">Home</g-link>
            </li>
            <li class="nav-item">
               <g-link to="/About">About</g-link>
            </li>
            <li class="nav-item">
              <g-link to="/post/">Sample Post</g-link>
            </li>
            <li class="nav-item">
               <g-link to="/contact">Contact</g-link>
            </li>
          </ul>
        </div>
      </div>
    </nav>

    <slot/>

        <!-- Footer -->
    <footer>
      <div class="container">
        <div class="row">
          <div class="col-lg-8 col-md-10 mx-auto">
            <ul class="list-inline text-center">
              <li class="list-inline-item">
                <a href="#">
                  <span class="fa-stack fa-lg">
                    <i class="fas fa-circle fa-stack-2x"></i>
                    <i class="fab fa-twitter fa-stack-1x fa-inverse"></i>
                  </span>
                </a>
              </li>
              <li class="list-inline-item">
                <a href="#">
                  <span class="fa-stack fa-lg">
                    <i class="fas fa-circle fa-stack-2x"></i>
                    <i class="fab fa-facebook-f fa-stack-1x fa-inverse"></i>
                  </span>
                </a>
              </li>
              <li class="list-inline-item">
                <a href="#">
                  <span class="fa-stack fa-lg">
                    <i class="fas fa-circle fa-stack-2x"></i>
                    <i class="fab fa-github fa-stack-1x fa-inverse"></i>
                  </span>
                </a>
              </li>
            </ul>
            <p class="copyright text-muted">
              Copyright &copy; Your Website 2020
            </p>
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>



<style></style>
