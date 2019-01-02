<template>
  <div id="app">
    <header-nav/>
    <div class="main-content columns is-fullheight">
      <side-menu/>
      <router-view/>
    </div>
  </div>
</template>

<script>
import HeaderNav from '@/components/HeaderNav'
import SideMenu from '@/components/SideMenu'

export default {
  name: 'App',
  components: {
    HeaderNav,
    SideMenu
  }
}
</script>

<style lang="sass">
$menu-item-active-background-color: hsl(171, 100%, 41%);
$menu-item-color: hsl(0, 0%, 100%);

@import '~bulma';
$fa-font-path: '~font-awesome/fonts/';
@import '~font-awesome/scss/font-awesome';

</style>
