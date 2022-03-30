<template>
  <div>
    <Banner />
    <Data-local />
    <img src="../css/images/line.png" alt="" class="divisoria" />
    <Form />
    <img src="../css/images/line.png" alt="" class="divisoria" />
    <Presentes />
    <img src="../css/images/line.png" alt="" class="divisoria" />
    <Contato />
  </div>
</template>

<script>
export default {
  name: "IndexPage",
};
</script>

<style>
body {
  /* background-image: url("../css/images/fundo.jpg"); */
  font-family: "josefin", sans-serif;
}

.divisoria {
  max-width: 100%;
  margin-top: 40px;
}
</style>
