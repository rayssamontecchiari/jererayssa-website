<template>
  <div class="wrapper-local">
    <div>
      <h2>É com grande alegria</h2>
      <p>Que te convidamos para nossa celebração de Casmento!</p>
    </div>
    <div>
      <p>Será no dia..</p>
      <b-calendar
        id="ex-disabled-readonly"
        :disabled="disabled"
        :readonly="readonly"
      ></b-calendar>
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
