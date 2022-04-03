<template>
  <div class="wrapper-local">
    <div>
      <h2>É com grande alegria</h2>
      <p>Que te convidamos para nossa celebração de Casamento!</p>
    </div>
    <div class="data-local">
      <div>
        <p>Será no dia..</p>
        <div class="calendario-wrapper">
          <div class="calendario">
            <h3 class="dia">31</h3>
            <p class="mes">Julho</p>
          </div>
        </div>
      </div>
      <div class="mapa-wrapper">
        <a
          href="https://www.google.com/maps/place/S%C3%ADtio+Recanto+da+Saudade/@-22.2566624,-42.4740366,17z/data=!4m13!1m7!3m6!1s0x0:0x9fbcc6d4c9629b25!2zMjLCsDE1JzI0LjAiUyA0MsKwMjgnMTguNyJX!3b1!8m2!3d-22.2566624!4d-42.4718479!3m4!1s0x97f3c2638a24e5:0x3cc171120c2d2959!8m2!3d-22.2561288!4d-42.4707382?hl=pt-BR"
          >E no sítio Recanto da Saudade</a
        >
        <a
          href="https://www.google.com/maps/place/S%C3%ADtio+Recanto+da+Saudade/@-22.2566624,-42.4740366,17z/data=!4m13!1m7!3m6!1s0x0:0x9fbcc6d4c9629b25!2zMjLCsDE1JzI0LjAiUyA0MsKwMjgnMTguNyJX!3b1!8m2!3d-22.2566624!4d-42.4718479!3m4!1s0x97f3c2638a24e5:0x3cc171120c2d2959!8m2!3d-22.2561288!4d-42.4707382?hl=pt-BR"
          ><img
            class="mapa"
            src="../css/images/sitio.jpeg"
            alt="Local do sítio"
        /></a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      state: "disabled",
      value: "2022/07/31",
      context: null,
    };
  },

  computed: {
    disabled() {
      return this.state === "disabled";
    },
    readonly() {
      return this.state === "readonly";
    },
  },

  methods: {
    onContext(ctx) {
      this.context = ctx;
    },
  },
};
</script>

<style>
.wrapper-local {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;

  width: 100vw;
  padding: 20px 0;
}

.calendario-wrapper {
  border: 1px solid #e0e0e0;
  border-radius: 5px;
  padding-top: 15px;
  background: rgb(165, 115, 165);
  display: block;
  width: 150px;
  margin: 0 auto;
}

.calendario {
  border: 1px solid #e0e0e0;
  border-radius: 5px;

  background: #fff;
}
.dia {
  /* border: 1px solid blue; */
  margin: 7px 0 0;
  font-size: 36px;
  display: flex;
  justify-content: center;
  align-items: center;
  line-height: 40px;
}
.mes {
  border-top: 0.5px solid #e0e0e0;
  margin: 0;
}

.mapa-wrapper {
  margin-top: 50px;
}

.mapa {
  display: block;
  width: 268px;
  height: 242px;
  object-fit: cover;
  margin-top: 20px;
}

h2,
h3,
p,
a {
  font-family: "josefin", sans-serif;
}

@media screen and (min-width: 800px) {
  .data-local {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 50px;
    align-items: flex-start;
  }
  .mapa-wrapper {
    margin-top: 0px;
  }
}
</style>
