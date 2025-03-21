<template>
  <q-header elevated class="header-floating">
    <q-toolbar class="q-toolbar-class">
      <div class="logo">
        <span class="logo-line1">CORTE</span>
        <span class="logo-line2">SUPREMO</span>
      </div>
      <div class="menu">
        <q-btn flat label="Home" to="/" />
        <q-btn flat label="Serviços" to="/servicos" />
        <q-btn flat label="Contato" to="/contato" />
      </div>
      <div class="action-button">
        <q-btn color="accent" label="Agendar Horario" to="/agendamento" />
      </div>
    </q-toolbar>
  </q-header>
</template>

<script setup></script>

<style scoped lang="scss">
.header-floating {
  padding: 1rem 0;
  background: transparent;
  z-index: 1000;
}

.q-toolbar-class {
  width: 1300px;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 100%;
}

.logo {
  display: flex;
  flex-direction: column;
  font-weight: bold;
  font-size: 1.5rem;
  line-height: 1;
  font-family: 'Hanken Grotesk';
}

.menu {
  flex: 1;
  display: flex;
  justify-content: center;
  gap: 1rem;
  font-family: 'Hanken Grotesk';
}

.action-button {
  display: flex;
  font-family: 'Hanken Grotesk';
}

.logo-line1 {
  font-size: 1.5rem;
}

.logo-line2 {
  font-size: 2rem;
}
</style>
