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

    <div class="check">
      <b-form-checkbox v-model="checked" name="check-button" switch>
        Sim, estarei lá
      </b-form-checkbox>
    </div>

    <div id="novo-nome"></div>

    <b-button
      type=""
      variant="secondary"
      class="btn-outros"
      @click="otherPeople"
    >
      Confirmar outra presença
    </b-button>

    <b-button
      type="submit"
      variant="secondary"
      class="btn-submit"
      @click="onSubmit"
    >
      Confirmar
    </b-button>
  </div>
</template>
<script>
// const novoNome = this.$el.querySelector("#novo-nome").value;

export default {
  data() {
    return {
      form: {
        name: "",
        age: "",
        checked: true,
      },
      checked: false,
    };
  },
  methods: {
    onSubmit() {
      console.log("On Submit");
      this.form.name = "";
      this.form.age = "";
      this.form.checked = "";
    },
    otherPeople() {
      // const inputname = "novo nome";
      // novoNome.innerHTML = inputname;
      // renderizar campo de nome outra vez
    },
  },
};
</script>

<style lang="css">
.form {
  text-align: center;

  display: flex;
  flex-direction: column;
  padding: 40px 10px 0;
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
