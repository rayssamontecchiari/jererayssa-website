<template>
  <div class="wrapper-local">
    <div>
      <h2>É com grande alegria</h2>
      <p>Que te convidamos para nossa celebração de Casaaaaaaamento!</p>
    </div>
    <div>
      <p>Será no dia..</p>
      <div class="calendario-wrapper">
        <div class="calendario">
          <h3 class="dia">31</h3>
          <p class="mes">julho</p>
        </div>
      </div>
      <!-- <b-calendar
        id="ex-disabled-readonly"
        :disabled="disabled"
        :readonly="readonly"
      ></b-calendar> -->
    </div>
    <div class="mapa-wrapper">
      <p>E no sítio Recanto da Saudade</p>
      <img
        class="mapa"
        src="../css/images/mapa-estatico.jpeg"
        alt="Local do sítio"
      />
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
.b-calendar-grid-help,
.b-calendar-nav,
.b-calendar-header {
  display: none !important;
}

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
}
</style>
