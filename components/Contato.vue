<template>
  <div class="contato-wrapper">
    <h2>Fale conosco:</h2>
    <div class="contatos-wrapper">
      <div>
        <p class="nome">Rayssa</p>
        <a href="tel:22997861096"> (22)99786-1096 </a>
      </div>
      <div>
        <p class="nome">Jeremias</p>
        <a href="tel:22998096470"> (22)99809-6470 </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.contato-wrapper {
  text-align: center;
  margin-top: 40px;

  font-family: "josefin", sans-serif;
}

.contatos-wrapper {
  display: flex;
  justify-content: space-around;
}

.nome {
  margin: 0;
}
</style>
