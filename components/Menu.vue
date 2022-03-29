<template>
  <div class="wrapper">
    <header class="cabecalho">
      <div class="container">
        <img class="logoHeader" src="../css/images/logo_header.png" href="/" />
        <!-- <b-nav small align="right" class="menu-wrapper">
          <b-nav-item active>Active</b-nav-item>
          <b-nav-item>Confirme sua presença</b-nav-item>
          <b-nav-item> Localização do evento</b-nav-item>
          <b-nav-item>Lista de presentes</b-nav-item>
        </b-nav> -->
      </div>
    </header>
  </div>
</template>

<script>
export default {};
</script>

<style>
/* .wrapper {
  position: sticky;
} */

.cabecalho {
  position: sticky;
  top: 0;
  right: 0;
  background: white;
  width: 100%;
}

.container {
  display: flex;
  max-height: 100px;
  /* border: 1px solid red; */
}

.logoHeader {
  max-height: 100px;
  object-fit: contain;
}

.menu-wrapper {
  display: flex;
  align-items: center;
}

a {
  color: black;
}
</style>
