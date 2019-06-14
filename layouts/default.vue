<template>
  <div>
    <nuxt/>

    <div id="wrapper">
      <div class="topbar">
        <div class="topbar-left">
          <a href="index.html" class="logo">
            <span>
              <img src="../static/images/Suzano_logo_Negativo.png" alt>
            </span>
            <i>
              <img src="../static/images/Suzano_Folha_Negativo.png" alt>
            </i>
          </a>
        </div>

        <nav class="navbar-custom">
          <ul class="list-unstyled topbar-right-menu float-right mb-0">
            <li class="dropdown notification-list">
              <a
                class="nav-link dropdown-toggle waves-effect waves-light nav-user"
                data-toggle="dropdown"
                href="#"
                role="button"
                aria-haspopup="false"
                aria-expanded="false"
              >
                <img src="../static/images/user.png" alt="user" class="rounded-circle">
                <span class="ml-1">
                  Anderson
                  <i class="mdi mdi-chevron-down"></i>
                </span>
              </a>

              <div class="dropdown-menu dropdown-menu-right profile-dropdown">
                <a href="javascript:void(0);" class="dropdown-item notify-item">
                  <i class="ti-lock"></i>
                  <span>Lock Screen</span>
                </a>

                <a href="javascript:void(0);" class="dropdown-item notify-item">
                  <i class="ti-power-off"></i>
                  <span>Logout</span>
                </a>
              </div>
            </li>
          </ul>

          <ul class="list-inline menu-left mb-0">
            <li class="float-left">
              <button class="button-menu-mobile open-left waves-light waves-effect">
                <i class="mdi mdi-menu"></i>
              </button>
            </li>
          </ul>
        </nav>
      </div>

      <Menu/>

      <div class="content-page">
        <div class="content">
          <div class="container-fluid">
            <div id="app"></div>
          </div>
          <div class="footer">
            <div>
              <strong>Portfólio de projetos</strong> - Suzano S/A 2019
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import Menu from "~/components/Menu.vue";

export default {
  components: {
    Menu
  },
   head() {
      return {
        title: 'Portfólio de projetos',
        meta: [          
          { hid: 'charset', name: 'charset', content: 'utf-8' },
          { hid: 'description', name: 'description', content: 'Portfólio de projetos digitais' },
          { hid: 'viewport', name: 'viewport', content: 'width=device-width, initial-scale=1' },
        ],
        script: [
          {src: '../static/js/jquery.min.js'},
          {src: '../static/js/popper.min.js'},
          {src: '../static/js/bootstrap.min.js'},
          {src: '../static/js/metisMenu.min.js'},
          {src: '../static/js/waves.js'},
          {src: '../static/js/jquery.slimscroll.js'},
          {src: '../static/js/jquery.core.js'},
          {src: '../static/js/jquery.app.js'}         
        ],
        link: [         
          {rel: 'stylesheet', href: '../static/css/bootstrap.min.css'},
          {rel: 'stylesheet', href: '../static/css/icons.css'},
          {rel: 'stylesheet', href: '../static/css/metismenu.min.css'},
          {rel: 'stylesheet', href: '../static/css/style.css'},
          {rel: 'stylesheet', href: '../static/css/site.css'}
        ]
      }
    },
};
</script>
<style>
</style>
