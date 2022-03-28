<template>
  <div>
    <header class="cabecalho">
      <div class="container">
        <img class="logoHeader" src="../css/images/logo_header.png" href="/" />
        <ul class="linksHeader">
          <li class="linkHeader">
            <a href="#presenca"> Confirme sua presença </a>
          </li>
          <li class="linkHeader">
            <a href="#local"> Localização do evento </a>
          </li>
          <li class="linkHeader">
            <a href="/contato"> Lista de presentes </a>
          </li>
        </ul>
      </div>
    </header>
  </div>
</template>

<script>
export default {};
</script>

<style>
.cabecalho {
  position: sticky;
  top: 0;
  right: 0;
  background: white;
}

.container {
  margin: 0 50px;
  display: flex;
  max-height: 100px;
  justify-content: space-between;
  /* border: 1px solid red; */
}

.logoHeader {
  max-height: 100px;
  object-fit: contain;
}

.linksHeader {
  display: flex;
  justify-content: space-between;

  /* border: 1px solid green; */
}

.linkHeader {
  list-style: none;
  display: flex;
  align-items: center;
  justify-content: center;

  font-family: "Lucida Sans", "Lucida Sans Regular", "Lucida Grande",
    "Lucida Sans Unicode", Geneva, Verdana, sans-serif;
  font-size: 22px;
  margin: 0 10px;

  pointer-events: all;

  /* border: 1px solid blue; */
}

a {
  text-decoration: none;
  color: black;
}
</style>
