<!-- eslint-disable -->
<template>
  <q-page id="addRoute">
    <!-- <div>Esta é a AddRoute</div> -->
    <q-toolbar class="text-white bg-teal-8">
      <q-toolbar-title> Adicionar rotas </q-toolbar-title>
      <q-btn to="/route/saved-routes" flat round dense icon="favorites" color="red" />
    </q-toolbar>

    <q-scroll-area class="q-pa-md form-style">
      <div class="text-h6 q-pb-md">Salve suas rotas favoritas!</div>

      <span class="text-body1 q-pd-md"> coloque um nome para esta rota </span>

      <q-input outlined stack-label label="Nome">
        <template v-slot:append>
          <q-icon name="close" />
        </template>
      </q-input>

      <div class="text-body1 q-pt-md">Salve suas rotas favoritas!</div>

      <q-input outlined stack-label label="De">
        <template v-slot:append>
          <q-icon name="close" />
        </template>
      </q-input>

      <q-input class="q-pt-md" outlined stack-label label="Para">
        <template v-slot:append>
          <q-icon name="close" />
        </template>
      </q-input>

      <div class="q-pt-md">
        <q-btn size="lg" class="full-width" color="black" label="Salvar a rota" />
      </div>
    </q-scroll-area>
  </q-page>
</template>

<script setup></script>

<style lang="scss">
#addRoute {
  .form-style {
    margin: 0 auto;
    height: calc(100vh - 180px);
    max-width: 500px;
  }
}
</style>
