<template>
  <q-layout>
    <q-header class="text-white bg-yellow-14" bordered>
      <q-toolbar class="">
        <q-toolbar-title class="text-logo">
           <q-avatar>
              <img src="../images/logofinal.png">
          </q-avatar>
          Artemis Academy
        </q-toolbar-title>
         <q-tabs v-model-tab active-color="" indicator-color="transparent">
           <q-route-tab label="inicio" to="/intro"/>
        <q-btn-dropdown auto-close stretch flat label="Matérias">
        <q-list class="">
                <q-route-tab label="Humanas" to=""/>
                  <q-separator/>
                <q-route-tab label="Natureza" to="/"/>
                  <q-separator/>
                <q-route-tab label="Matemática" to="/"/>
                  <q-separator/>
                <q-route-tab label="Linguagens" to="/"/>
                  <q-separator/>
                <q-route-tab label="Concursos" to="/"/>
                  <q-separator/>
                <q-route-tab label="Faculdade" to="/"/>
          </q-list>
        </q-btn-dropdown>
        <q-separator/>
        <q-btn-dropdown auto-close stretch flat label="Complementares">
        <q-list class="">
                <q-route-tab label="Educação financeira" to="/intro"/>
                  <q-separator/>
                <q-route-tab label="Sustentabilidade" to="/"/>
                  <q-separator/>
                <q-route-tab label="Produção Digital" to="/"/>
                  <q-separator/>
                <q-route-tab label="Saúde" to="/"/>
                  <q-separator/>
                <q-route-tab label="Política" to="/"/>
                  <q-separator/>
                <q-route-tab label="Linguistica" to="/"/>
                  <q-separator/>
                <q-route-tab label="Avulsos" to="/"/>
          </q-list>
        </q-btn-dropdown>
        <q-separator/>
        <q-btn-dropdown auto-close stretch flat label="Desenvolvimento">
        <q-list class="">
                <q-route-tab label="Pessoal" to="/"/>
                  <q-separator/>
                <q-route-tab label="Profissional" to="/"/>
          </q-list>
        </q-btn-dropdown>
        <q-separator/>
        <!--<q-route-tab label="Enviar" to="/enviar"/>-->
      </q-tabs>
      </q-toolbar>
    </q-header>

    <q-page-container class="">
      <router-view />
    </q-page-container>
  </q-layout>
</template>
<script>
</script>
<style lang="sass">
  .q-toolbar__title
    font-size: 30px
      text-align: center
      font-family: 'Grand Hotel', cursive
  .background
    background-color: #FFD700
  .text-logo
    font-family: 'Grand Hotel', 'cursive'
</style>
