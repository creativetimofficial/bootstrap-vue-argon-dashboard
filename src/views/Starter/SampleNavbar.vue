<template>
  <base-nav
    container-classes="container-fluid"
    class="navbar-top border-bottom navbar-expand"
    :class="$route.meta.navbarClasses ? $route.meta.navbarClasses : 'bg-success navbar-dark'"
    type=""
  >
    <!-- Search form -->
    <b-form class="navbar-search form-inline mr-sm-3"
          :class="$route.meta.searchClasses ? $route.meta.searchClasses : 'navbar-search-light'"
          id="navbar-search-main">
      <b-form-group class="mb-0">
        <b-input-group class="input-group-alternative input-group-merge">
          <div class="input-group-prepend">
            <span class="input-group-text"><i class="fas fa-search"></i></span>
          </div>
          <b-form-input placeholder="Search" type="text"></b-form-input>
        </b-input-group>
      </b-form-group>
      <button type="button" class="close" data-action="search-close" data-target="#navbar-search-main" aria-label="Close">
        <span aria-hidden="true">×</span>
      </button>
    </b-form>
    <!-- Navbar links -->
    <b-navbar-nav class="align-items-center ml-md-auto">
      <!-- This item dont have <b-nav-item> becouse they add class 'nav-link' which is not needed here -->
      <li class="nav-item d-xl-none">
        <!-- Sidenav toggler -->
        <div class="pr-3 sidenav-toggler sidenav-toggler-dark"
             @click="toggleSidebar">
          <div class="sidenav-toggler-inner">
            <i class="sidenav-toggler-line"></i>
            <i class="sidenav-toggler-line"></i>
            <i class="sidenav-toggler-line"></i>
          </div>
        </div>
      </li>
      <!-- This item dont have <b-nav-item> because item have data-action/data-target on tag <a>, wich we cant add -->
      <li class="nav-item d-sm-none">
        <a class="nav-link" href="#" data-action="search-show" data-target="#navbar-search-main">
          <i class="ni ni-zoom-split-in"></i>
        </a>
      </li>
    </b-navbar-nav>
    <b-navbar-nav class="align-items-center ml-auto ml-md-0">
      <b-nav-item-dropdown right>
        <b-dropdown-item  class="pr-0" href="#" >
          <b-media no-body class="align-items-center">
                  <span class="avatar avatar-sm">
                    <b-img alt="Image placeholder" rounded="circle" src="img/theme/team-4.jpg" />
                  </span>
            <b-media-body class="ml-2 d-none d-lg-block">
              <span class="mb-0 text-sm  font-weight-bold">John Snow</span>
            </b-media-body>
          </b-media>
        </b-dropdown-item>
        <b-dropdown>
          <b-dropdown-header class="noti-title">
            <h6 class="text-overflow m-0">Welcome!</h6>
          </b-dropdown-header >
          <b-dropdown-item href="#!">
            <i class="ni ni-single-02"></i>
            <span>My profile</span>
          </b-dropdown-item>
          <b-dropdown-item href="#!">
            <i class="ni ni-settings-gear-65"></i>
            <span>Settings</span>
          </b-dropdown-item>
          <b-dropdown-item href="#!">
            <i class="ni ni-calendar-grid-58"></i>
            <span>Activity</span>
          </b-dropdown-item>
          <b-dropdown-item href="#!">
            <i class="ni ni-support-16"></i>
            <span>Support</span>
          </b-dropdown-item>
          <div class="dropdown-divider"></div>
          <b-dropdown-item href="#!">
            <i class="ni ni-user-run"></i>
            <span>Logout</span>
          </b-dropdown-item>
        </b-dropdown>
      </b-nav-item-dropdown>
    </b-navbar-nav>
  </base-nav>
</template>
<script>
  import { CollapseTransition } from 'vue2-transitions';
  import { BaseNav, Modal } from '@/components';

  export default {
    components: {
      CollapseTransition,
      BaseNav,
      Modal
    },
    computed: {
      routeName() {
        const { name } = this.$route;
        return this.capitalizeFirstLetter(name);
      },
      isRTL() {
        return this.$rtl.isRTL;
      }
    },
    data() {
      return {
        activeNotifications: false,
        showMenu: false,
        searchModalVisible: false,
        searchQuery: ''
      };
    },
    methods: {
      capitalizeFirstLetter(string) {
        return string.charAt(0).toUpperCase() + string.slice(1);
      },
      toggleNotificationDropDown() {
        this.activeNotifications = !this.activeNotifications;
      },
      closeDropDown() {
        this.activeNotifications = false;
      },
      toggleSidebar() {
        this.$sidebar.displaySidebar(!this.$sidebar.showSidebar);
      },
      hideSidebar() {
        this.$sidebar.displaySidebar(false);
      }
    }
  };
</script>
<style scoped>
  .top-navbar {
    top: 0px;
  }
</style>
