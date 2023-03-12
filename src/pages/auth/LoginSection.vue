<template>
  <div>Esta é a LoginSection</div>
  <q-page id="loginPage">
    <q-toolbar class="text-white bg-teal-8">
      <q-toolbar-title>Login</q-toolbar-title>
    </q-toolbar>

    <q-scroll-area class="form-style">
      <div class="text-h6 text-center q-pt-md">
        <q-img src="favicon.ico" height="60px" width="60px" />
        <div>Carregando mapa EV</div>
      </div>

      <div class="q-pa-md q-gutter-md">
        <div class="text-center">Registrar e obter características extras</div>

        <q-input outlined stack-label label="Email">
          <template v-slot:append>
            <q-icon name="close" />
          </template>
        </q-input>

        <q-input outlined stack-label label="Senha">
          <template v-slot:append>
            <q-icon name="close" />
          </template>
        </q-input>

        <div>
          <q-btn color="black" size="lg" class="full-width" label="Registrar" />
        </div>

        <div class="q-px-md q-mt-xl text-center">
          <div class="q-mb-md no-account">Ainda não tem uma conta ?</div>
          <q-btn color="teal" outline rounded to="/auth/register" size="15px">Registre aqui</q-btn>
        </div>
      </div>
    </q-scroll-area>
  </q-page>
</template>

<script setup></script>

<style lang="scss">
#loginPage {
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
