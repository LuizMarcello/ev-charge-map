<template>
  <div>Esta é a MyDetails</div>
  <q-page id="myDetails">
    <q-toolbar class="text-white bg-teal-8">
      <q-toolbar-title>Meus detalhes</q-toolbar-title>
    </q-toolbar>
    <q-scroll-area class="form-style">
      <!--  <div class="text-h6 text-center q-pt-md">
        <q-img src="favicon.ico" height="60px" width="60px" />
        <div>Carregando mapa EV</div>
      </div> -->
      <div class="q-pa-md q-gutter-md">
        <div class="text-h6">Atualize seus detalhes!</div>

        <q-input outlined stack-label label="Nome">
          <template v-slot:append>
            <q-icon name="close" />
          </template>
        </q-input>

        <q-input outlined stack-label label="Sobrenome">
          <template v-slot:append>
            <q-icon name="close" />
          </template>
        </q-input>

        <div class="text-yellow-10 text-bold q-mt-md">
          Nota: Este email é somente leitura
        </div>

        <q-input outlined stack-label readonly label="Email" />

        <div>
          <q-btn
            color="black"
            size="lg"
            class="full-width"
            label="Atualizar os detalhes"
          />
        </div>
      </div>
    </q-scroll-area>
  </q-page>
</template>

<script setup></script>

<style lang="scss">
#myDetails {
  .form-style {
    margin: 0 auto;
    height: calc(100vh - 180px);
    max-width: 500px;
  }
  .no-account {
    font-size: 17px;
  }
}
</style>
