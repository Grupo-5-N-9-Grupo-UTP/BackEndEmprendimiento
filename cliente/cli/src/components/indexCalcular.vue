<template>
  <div class="container">
    <span class="big-circle"></span>
    <img src="img/007-hourglass.png" class="square" alt="" />
    <div class="form-invertida">
      <form action="indexContactenos.html" method="POST" autocomplete="off">
        <h3 class="title">Calcula tu Rentabilidad</h3>
        <div class="input-container">
          <input
            type="text"
            id="name-emprendimiento"
            class="input"
            placeholder="Nombre Emprendimiento"
            required
          />
          <!-- <label for="">Nombre Emprendimiento</label> -->
          <span>Nombre Emprendimiento</span>
        </div>
        <div class="input-container">
          <input
            type="text"
            id="tipo-negocio"
            class="input"
            placeholder="Tipo de Negocio"
            required
          />
          <span>Tipo de Negocio</span>
        </div>
        <div class="input-container">
          <input
            type="text"
            id="ingresos"
            class="input"
            placeholder="Ingresos"
            required
          />
          <span>Ingresos</span>
          <span class="tooltip"
            >Ingresos para el periodo a analizar (mensual - trimestral -
            anual)</span
          >
        </div>
        <div class="input-container">
          <input
            type="text"
            id="costo_bienes_vendidos"
            class="input"
            placeholder="Costo de Bienes Vendidos"
            required
          />
          <span>Costo de Bienes Vendidos</span>
          <span class="tooltip"
            >Costos de bienes vendidos = Inventario inicial + Compras realizadas
            durante el periodo de tiempo – Inventario final.</span
          >
        </div>
        <div class="input-container">
          <input
            type="text"
            id="ganancias_operativas"
            class="input"
            placeholder="Ganancias Operativos"
            required
          />
          <span>Ganancias Operativos</span>
          <span class="tooltip"
            >Ganancias operativas: Ingresos – costo de bienes vendidos – gastos
            operativos – depreciación – amortización.</span
          >
        </div>
        <div class="input-container">
          <input
            type="text"
            id="gastos_totales"
            class="input"
            placeholder="Gastos Totales"
            required
          />
          <span>Gastos Totales</span>
          <span class="tooltip"
            >Todos los gastos incurridos por la empresa</span
          >
        </div>

        <input
          type="button"
          value="Calcular"
          class="btn"
          @click="calculate()"
        />
      </form>

      <div class="contact-form-invertida">
        <span class="circle one"></span>
        <span class="circle two"></span>

        <div class="contact-info">
          <h3 class="title">Ejemplo Indice de Rentabilidad</h3>
          <p class="text">
            <img src="../assets/img/Nada.png" class="image" />
          </p>
          <div class="info">
            <div class="informacion">
              <input
                type="button"
                value="Ver Grafico"
                class="btn-invertido"
                href="#"
              />
            </div>
            <br />
            <div class="informacion">
              <br />
              <a
                target="_blank"
                style="text-decoration: none"
                class="btn-invertido"
                href="https://www.caminofinancial.com/es/como-calcular-los-indices-de-rentabilidad-de-tu-empresa/"
                >Quizá te interese</a
              >
            </div>
          </div>

          <div class="social-media">
            <p>Conéctate con nosotros :</p>
            <div class="social-icons">
              <a target="_blank" href="https://www.facebook.com/">
                <img src="../assets/img/043-facebook-1.png" class="icon2" />
              </a>
              <a target="_blank" href="https://twitter.com/">
                <img src="../assets/img/013-twitter-1.png" class="icon2" />
              </a>
              <a target="_blank" href="https://instagram.com/">
                <img src="../assets/img/034-instagram.png" class="icon2" />
              </a>
              <a target="_blank" href="https://www.linkedin.com/">
                <img src="../assets/img/031-linkedin.png" class="icon2" />
              </a>
              <a
                target="_blank"
                href="https://github.com/Grupo-5-N-9-Grupo-UTP"
              >
                <img src="../assets/img/039-github.png" class="icon2" />
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script
    src="https://kit.fontawesome.com/64d58efce2.js"
    crossorigin="anonymous">
</script>

<script>
import "../assets/scripts/app.js";
export default {
  name: "index-calcular",
  props: {
    msg: String,
  },

  methods: {
    calculate: function () {
      var ingresos = document.getElementById("ingresos");
      var costo__bienes_vendidos = document.getElementById(
        "costo_bienes_vendidos"
      );
      var ganancias_operativas = document.getElementById("ganacias_operativas");
      var gastos_totales = document.getElementById("gastos_totales");

      var ganancias_netas = ingresos - gastos_totales;

      var m_ganancia_bruta =
        ((ingresos - costo__bienes_vendidos) / ingresos) * 100;
      var m_ganancia_neta = (ganancias_netas / ingresos) * 100;
      var m_ganancia_operativa = (ganancias_operativas / ingresos) * 100;
    },
  },
};
</script>

<style>
@import "../assets/styles/style.css";
</style>
