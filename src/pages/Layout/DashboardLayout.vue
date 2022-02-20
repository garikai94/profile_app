<template>
  <div class="wrapper" :class="{ 'nav-open': $sidebar.showSidebar }">
    <notifications></notifications>

    <side-bar
      :sidebar-item-color="sidebarBackground"
      :sidebar-background-image="sidebarBackgroundImage"
    >
      <mobile-menu slot="content"></mobile-menu>
      <sidebar-link v-scroll-to="'#education'" to="/user">
        <md-icon>school</md-icon>
        <p>Education</p>
      </sidebar-link>
      <sidebar-link v-scroll-to="'#portfolio'" to="user">
        <md-icon>portfolio</md-icon>
        <p>Portfolio</p>
      </sidebar-link>
      <sidebar-link v-scroll-to="'#about'" to="user">
        <md-icon>about</md-icon>
        <p>About</p>
      </sidebar-link>
      <sidebar-link v-scroll-to="'#contact'" to="user">
        <md-icon>contact</md-icon>
        <p>Contact</p>
      </sidebar-link>

     <!-- <sidebar-link to="/user">
        <md-icon>person</md-icon>
        <p>User Profile</p>
      </sidebar-link>
      <sidebar-link to="/table">
        <md-icon>content_paste</md-icon>
        <p>Table list</p>
      </sidebar-link>
      <sidebar-link to="/typography">
        <md-icon>library_books</md-icon>
        <p>Typography</p>
      </sidebar-link>
      <sidebar-link to="/icons">
        <md-icon>bubble_chart</md-icon>
        <p>Icons</p>
      </sidebar-link>
      <sidebar-link to="/maps">
        <md-icon>location_on</md-icon>
        <p>Maps</p>
      </sidebar-link>
      <sidebar-link to="/notifications">
        <md-icon>notifications</md-icon>
        <p>Notifications</p>
      </sidebar-link>
      <sidebar-link to="/upgrade" class="active-pro">
        <md-icon>unarchive</md-icon>
        <p>Upgrade to PRO</p>
      </sidebar-link>-->
    </side-bar>

    <div class="main-panel">
      <top-navbar></top-navbar>

      <fixed-plugin
        :color.sync="sidebarBackground"
        :image.sync="sidebarBackgroundImage"
      >
      </fixed-plugin>

      <dashboard-content> </dashboard-content>

      <content-footer v-if="!$route.meta.hideFooter"></content-footer>
    </div>
  </div>
</template>

<script>
//import TopNavbar from "./TopNavbar.vue";
import ContentFooter from "./ContentFooter.vue";
import DashboardContent from "./Content.vue";
import MobileMenu from "@/pages/Layout/MobileMenu.vue";
//import FixedPlugin from "./Extra/FixedPlugin.vue";

export default {
  components: {
    /*TopNavbar,*/
    DashboardContent,
    ContentFooter,
    MobileMenu,
   /* FixedPlugin,*/
  },
  data() {
    return {
      sidebarBackground: "silver",
      sidebarBackgroundImage: require("@/assets/img/faces/pc.jpg"),
    };
  },
};
</script>
