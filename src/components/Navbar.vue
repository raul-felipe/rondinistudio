<template>
  <b-navbar class="navbar" toggleable="lg" type="light" variant="light">
    <b-navbar-brand href="#" class="col-sm-4" >
        <img src="../assets/logo/Logo Rondini (Sem Fundo 2).png" width="100" height="100%" alt="">
    </b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" class="nav-collapse" is-nav >
      <b-navbar-nav class="col-sm-6 justify-content-center">
        <b-nav-item href="#"><h3>Sobre</h3></b-nav-item>
        <b-nav-item href="#" disabled><h3>Projetos</h3></b-nav-item>
      </b-navbar-nav>

      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto col-sm-6 justify-content-end" right>

        <b-navbar-brand href="https://www.behance.net/rondinistudio" target="_blank" >
            <img src="../assets/behance.png" width="35" height="35" >
        </b-navbar-brand>

        <b-navbar-brand href="https://www.instagram.com/rondini.studio/" target="_blank" >
            <img src="../assets/instagram.png" width="35" height="35">
        </b-navbar-brand>

      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</template>

<style>

</style>