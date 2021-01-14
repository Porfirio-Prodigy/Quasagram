<template>
  <q-layout view="lHh Lpr lFf">
    <q-header class="text-grey-10 bg-white" bordered>
      <q-toolbar class="constrain">
        <q-btn flat round dense icon="eva-camera-outline" to="/camera" size="18px" class="large-screen-only q-mr-sm"/>
        <q-separator vertical spaced class="large-screen-only"/> <!--SEPARATOR-->
        <q-toolbar-title class="text-bold">
          Quasagram
        </q-toolbar-title>
        <q-btn flat round dense icon="eva-home-outline" to="/" size="18px" class="large-screen-only"/>
      </q-toolbar>
    </q-header>

    <q-footer class="bg-white small-screen-only" bordered>
      <q-tabs
        v-model="tab" class="text-grey-10" active-color="primary" indicator-color="transparent">
        <q-route-tab icon="eva-home-outline" to="/" />
        <q-route-tab icon="eva-camera-outline" to="/camera" />
      </q-tabs>
    </q-footer>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
export default {
  name: 'MainLayout',

  data () {
    return {

    }
  }
}
</script>

<style lang="sass">
  .q-toolbar
    @media (min-width: $breakpoint-sm-min)
      height: 77px
  .q-toolbar__title
    font-size: 30px
    @media (max-width: $breakpoint-xs-max)
      text-align: center
    font-family: 'Grand Hotel', cursive
  .q-footer
    .q-tab__icon
      font-size: 30px
</style>
