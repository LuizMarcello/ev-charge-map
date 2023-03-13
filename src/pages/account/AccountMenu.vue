<template>
  <div>Esta é a AccountMenu</div>
  <q-page id="accountMenu">
    <q-toolbar class="text-white bg-teal-8">
      <q-toolbar-title>Conta</q-toolbar-title>
    </q-toolbar>

    <div class="text-h6 text-center q-pa-xl">
      <q-avatar size="60px" color="green">LM</q-avatar>
      <div>Luiz Marcello</div>
    </div>

    <div class="menu">
      <q-separator inset />
      <q-list class="q-mx-md">
        <q-item clickable v-ripple>
          <q-item-section avatar>
            <q-avatar rounded color="primary" text-color="white" icon="account_box" />
          </q-item-section>

          <q-item-section class="text-size">Detalhes da conta</q-item-section>

          <q-item-section side>
            <q-icon name="arrow_right" size="35px" />
          </q-item-section>
        </q-item>
      </q-list>

      <q-separator inset />

      <q-list class="q-mx-md">
        <q-item clickable v-ripple>
          <q-item-section avatar>
            <q-avatar rounded color="red" text-color="white" icon="logout" />
          </q-item-section>

          <q-item-section class="text-size">Logout</q-item-section>

          <q-item-section side>
            <q-icon name="arrow_right" size="35px" />
          </q-item-section>
        </q-item>
      </q-list>

      <q-separator inset />
    </div>
  </q-page>
</template>

<script setup></script>

<style lang="scss">
#accountMenu {
  .menu {
    margin: 0 auto;
    max-width: 500px;
  }

  .text-size {
    font-size: 18px;
  }
}
</style>
