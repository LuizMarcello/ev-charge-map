<!-- eslint-disable -->
<template>
  <q-layout>
    <q-header class="bg-teal">
      <q-toolbar>
        <q-toolbar-title> Ev Carregando mapas </q-toolbar-title>

        <q-btn flat round dense icon="login" />
      </q-toolbar>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>

    <q-footer elevated>
      <q-tabs class="text-light bg-teal">
        <q-tab name="/map" icon="explore" label="Mapa" />
        <q-tab name="/route" icon="directions" label="Rotas" />
        <q-tab name="movies" icon="login" label="Auth" />
      </q-tabs>
    </q-footer>
  </q-layout>
</template>

<script setup></script>
