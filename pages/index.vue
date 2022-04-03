<template>
  <div>
    <Banner />
    <Data-local />
    <div class="divisoria">
      <img src="../css/images/line.png" alt="" />
    </div>
    <Form />
    <div class="divisoria">
      <img src="../css/images/line.png" alt="" />
    </div>
    <Presentes />
    <div class="divisoria">
      <img src="../css/images/line.png" alt="" />
    </div>
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
  width: 100%;
  margin: 40px 0 0;

  display: flex;
  justify-content: center;
}

.divisoria img {
  max-width: 150px;
  margin: 0 auto;
}

a {
  color: black;
}
</style>
