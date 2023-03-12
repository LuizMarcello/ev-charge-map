<template>
  <q-page id="savedRoutes">
    <!-- <div>Esta é a SavedRoutes</div> -->
    <q-toolbar class="text-white bg-teal-8">
      <q-toolbar-title> Rotas salvas </q-toolbar-title>
      <q-btn flat round dense icon="add" size="20px" />
    </q-toolbar>

    <div class="section-title">
      <div class="text-h6 q-mx-sm">Selecione uma das suas rotas salvas!</div>
    </div>

    <div class="text-center q-pt-lg">
      <q-btn flat round dense icon="add_circle_outline" size="33px" />
      <div class="text-h6">Adicionas algumas rotas!</div>
      <div class="q-pa-md info">
        Aqui é onde você pode adicionar suas viagens favoritas ou comuns
      </div>
    </div>

    <q-scroll-area class="list">
      <q-list>
        <q-item>
          <q-item-section top avatar>
            <q-avatar color="green" text-color="white" icon="directions" />
          </q-item-section>

          <q-item-section>
            <q-item-label>Uma nova rodovia legal</q-item-label>
            <q-item-label caption>
              <div class="q-px-sm"><b>De</b>: Esta seção é o inicio</div>
              <div class="q-px-sm"><b>Para</b>: Esta seção é para onde</div>
              <div class="q-px-sm"><b>Raio de busca</b>: 3</div>
            </q-item-label>
          </q-item-section>

          <q-item-section side bottom>
            <q-btn class="q-ma-sm" label="Ir para o mapa" color="green" size="sm" />
            <q-btn class="q-mx-sm" label="Deletar" color="red" size="sm" />
          </q-item-section>
        </q-item>
      </q-list>
    </q-scroll-area>
  </q-page>
</template>

<script setup></script>

<style lang="scss">
#savedRoutes {
  .section-title {
    padding: 12px 10px 8px 10px;
    max-width: 500px;
    margin: 0 auto;
  }
  .info {
    font-size: 16px;
  }
  .list {
    margin: 0 auto;
    height: calc(100vh - 250px);
    max-width: 500px;
  }
}
</style>
