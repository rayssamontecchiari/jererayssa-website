<template>
  <div class="form">
    <h2>Confirme sua presença</h2>

    <b-form-group label-for="name" class="name">
      <b-form-input
        id="name"
        v-model="form.name"
        type="text"
        placeholder="Seu nome"
        required
      />
    </b-form-group>

    <div class="novo-nome">
      <b-form-group label-for="name" class="name">
        <b-form-input
          id="name"
          v-model="form.name"
          type="text"
          placeholder="Nome"
          required
        />
      </b-form-group>
    </div>

    <b-button
      type=""
      variant="secondary"
      class="btn-outros"
      @click="otherPeople"
    >
      Confirmar presença de outra pessoa
    </b-button>

    <b-button
      type="submit"
      variant="secondary"
      class="btn-submit"
      @click="onSubmit"
    >
      Confirmar presença
    </b-button>
  </div>
</template>
<script>
export default {
  data() {
    return {
      form: {
        name: "",
      },
    };
  },
  methods: {
    onSubmit() {
      console.log("On Submit");
      this.form.name = "";
    },
    otherPeople(elemento) {
      elemento.style.display = "block";
    },
  },
};
</script>

<style lang="css">
.novo-nome {
  display: none;
}

.form {
  text-align: center;
  font-family: "josefin", sans-serif;

  display: flex;
  flex-direction: column;
  padding: 60px 10px 20px;
}
.btn-submit,
.btn-submit:after {
  background-color: #482763;
  width: 100%;
  outline: none;
  border: none;
}

.check {
  margin-bottom: 10px;
}

.custom-control-input:checked ~ .custom-control-label::before {
  border-color: #877199;
  background-color: #877199;
}

.btn-outros {
  margin-bottom: 10px;
  width: 100%;
  background-color: #877199;
  outline: none;
  border: none;
}
</style>
