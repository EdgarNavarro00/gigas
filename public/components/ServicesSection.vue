<template>
  <section id="services" class="page-section">
    <div class="container">
      <div class="text-center">
        <h2 class="section-heading text-uppercase">Servicios</h2>
        <h3 class="section-subheading text-muted">
          Creamos Soluciones Integrales de Gas Natural y Gas L.P.
        </h3>
      </div>
      <div class="row text-center">
        <div class="col-md-12">
          <h4 class="my-3">Ingeniería BIM Gas NATURAL y GAS L.P.</h4>
          <ul class="text-muted no-marks">
            <li>Ingeniería BIM</li>
            <li>Memoria de cálculo</li>
            <li>Memoria descriptiva</li>
            <li>Levantamientos</li>
            <li>Cuantificación</li>
            <li>Catálogo de conceptos</li>
            <li>Presupuesto Desglosado</li>
          </ul>
        </div>
      </div>
      <div class="row">
        <div class="column">
          <img src="~/assets/img/gallery/bim-1.jpeg" />
          <img src="~/assets/img/gallery/bim-5.jpeg" />
        </div>
        <div class="column">
          <img src="~/assets/img/gallery/bim-2.jpeg" />
          <img src="~/assets/img/gallery/bim-6.jpeg" />
        </div>
        <div class="column">
          <img src="~/assets/img/gallery/bim-3.jpeg" />
          <img src="~/assets/img/gallery/bim-7.jpeg" />
        </div>
        <div class="column">
          <img src="~/assets/img/gallery/bim-4.jpeg" />
          <img src="~/assets/img/gallery/bim-8.jpeg" />
        </div>
      </div>
      <div class="row text-center">
        <div class="col-md-12">
          <h4 class="my-3">Instalación de Gas NATURAL y GAS L.P.</h4>
          <ul class="text-muted no-marks">
            <li>Instalaciones Industriales</li>
            <li>Instalaciones Comerciales</li>
            <li>Instalaciones Residenciales</li>
            <li>Mantenimientos</li>
          </ul>
        </div>
      </div>
      <div class="row">
        <div class="column">
          <img src="~/assets/img/gallery/inst-01.jpg" />
          <img src="~/assets/img/gallery/inst-05.jpg" />
        </div>
        <div class="column">
          <img src="~/assets/img/gallery/inst-02.jpg" />
          <img src="~/assets/img/gallery/inst-06.jpg" />
        </div>
        <div class="column">
          <img src="~/assets/img/gallery/inst-03.jpg" />
          <img src="~/assets/img/gallery/inst-07.jpg" />
        </div>
        <div class="column">
          <img src="~/assets/img/gallery/inst-04.jpg" />
          <img src="~/assets/img/gallery/inst-08.png" />
        </div>
      </div>
    </div>
  </section>
</template>
<style>
.no-marks {
  list-style-type: none;
}

.row {
  display: flex;
  flex-wrap: wrap;
  padding: 0 4px;
}

/* Create four equal columns that sits next to each other */
.column {
  flex: 25%;
  max-width: 25%;
  padding: 0 4px;
}

.column img {
  margin-top: 8px;
  vertical-align: middle;
  width: 100%;
}

/* Responsive layout - makes a two column-layout instead of four columns */
@media screen and (max-width: 800px) {
  .column {
    flex: 50%;
    max-width: 50%;
  }
}

/* Responsive layout - makes the two columns stack on top of each other instead of next to each other */
@media screen and (max-width: 600px) {
  .column {
    flex: 100%;
    max-width: 100%;
  }
}
</style>