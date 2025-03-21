<template>
  <div class="banner">
    <q-img src="/images/barber-banner.jpg" class="banner-img" ratio="16/9">
      <div class="banner-overlay">
        <q-toolbar class="q-pa-none q-mb-md">
          <q-toolbar-title class="text-white text-uppercase lk-toolbar-class">
            <p class="text-overline-toolbar">Desde 1999</p>
            <p>A Barbearia dos</p>
            <span class="highlight-text">Homens</span>
          </q-toolbar-title>
        </q-toolbar>
        <div class="card-container">
          <q-card class="q-pa-md text-center transparent-card">
            <q-card-section>
              <p class="text-white text-subtitle1">
                Renove seu estilo, cuide da sua barba e sinta-se no controle. Aqui, cada corte é uma
                experiência única!
              </p>
            </q-card-section>
            <q-card-actions align="center">
              <q-btn color="white" text-color="white" outline label="Ver Mais" size="lg" />
            </q-card-actions>
          </q-card>
        </div>
      </div>
    </q-img>
    <div class="banner-inclined">
      <q-toolbar>
        <q-toolbar-title class="text-uppercase">
          <p class="text-title-banner-inclined">Força, estilo e respeito</p>
        </q-toolbar-title>
      </q-toolbar>
    </div>
  </div>
</template>

<style scoped lang="scss">
.banner {
  width: 100%;
  height: 80vh;
  font-family: 'Hanken Grotesk';
}

.banner-img {
  width: 100%;
  height: 100%;
}

.banner-overlay {
  padding: 2rem;
  border-radius: 10px;
  text-align: center;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  background: transparent;
}

.text-overline-toolbar {
  font-size: 0.8rem;
  line-height: 1rem;
  font-weight: 200;
}

.lk-toolbar-class {
  font-size: 3.75rem;
  line-height: 3.75rem;
  font-weight: 400;
}

.highlight-text {
  text-align: center;
  -webkit-text-stroke-width: 2px;
  -webkit-text-stroke-color: #ff7b42;
  color: transparent;
  font-size: 3.75rem;
  font-style: normal;
  font-weight: 400;
  line-height: 3.75rem;
  letter-spacing: 0.0625rem;
  text-transform: uppercase;
}

.card-container {
  flex: 1;
  display: flex;
  justify-content: center;
  align-items: center;
}

.transparent-card {
  background: transparent;
  box-shadow: none;
}

.banner-inclined {
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  background: #ff7b42;
  padding: 1rem 0rem;
  transform: skewY(-3deg);
  margin-top: -3rem;
}

.text-title-banner-inclined {
  font-family: 'Bungee Hairline';
  -webkit-text-stroke-width: 2px;
  -webkit-text-stroke-color: #000;
  font-size: 4rem;
}
</style>
