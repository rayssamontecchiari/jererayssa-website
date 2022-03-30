<template>
  <div class="wrapper-banner">
    <b-container fluid class="p-4 banner-wrapper">
      <b-row>
        <b-col>
          <b-img
            fluid
            src="../css/images/casal.jpeg"
            alt="Image 1"
            class="imagem-banner"
          >
          </b-img>
        </b-col>
        <b-col>
          <b-img
            fluid
            src="../css/images/foto1.jpg"
            alt="Image 2"
            class="imagem-banner"
          ></b-img>
        </b-col>
        <b-col>
          <b-img
            fluid
            src="../css/images/foto.PNG"
            alt="Image 3"
            class="imagem-banner"
          ></b-img>
        </b-col>
        <b-col>
          <b-img
            fluid
            src="../css/images/foto1.jpg"
            alt="Image 2"
            class="imagem-banner"
          ></b-img>
        </b-col>
      </b-row>
      <b-row>
        <b-col>
          <b-img
            fluid
            src="../css/images/foto2.jpg"
            alt="Image 3"
            class="imagem-banner"
          ></b-img>
        </b-col>
        <b-col>
          <b-img
            fluid
            src="../css/images/foto3.jpg"
            alt="Image 3"
            class="imagem-banner"
          ></b-img>
        </b-col>
        <b-col>
          <b-img
            fluid
            src="../css/images/foto4.jpg"
            alt="Image 3"
            class="imagem-banner"
          ></b-img>
        </b-col>
        <b-col>
          <b-img
            fluid
            src="../css/images/foto3.jpg"
            alt="Image 3"
            class="imagem-banner"
          ></b-img>
        </b-col>
      </b-row>
      <b-row>
        <b-col>
          <b-img
            fluid
            src="../css/images/foto5.JPG"
            alt="Image 3"
            class="imagem-banner"
          ></b-img>
        </b-col>
        <b-col>
          <b-img
            fluid
            src="../css/images/foto6.jpg"
            alt="Image 3"
            class="imagem-banner"
          ></b-img>
        </b-col>
        <b-col>
          <b-img
            fluid
            src="../css/images/banner_1.jpeg"
            alt="Image 3"
            class="imagem-banner"
          ></b-img>
        </b-col>
        <b-col>
          <b-img
            fluid
            src="../css/images/foto6.jpg"
            alt="Image 3"
            class="imagem-banner"
          ></b-img>
        </b-col>
      </b-row>
      <b-row>
        <b-col>
          <b-img
            fluid
            src="../css/images/foto2.jpg"
            alt="Image 3"
            class="imagem-banner"
          ></b-img>
        </b-col>
        <b-col>
          <b-img
            fluid
            src="../css/images/foto3.jpg"
            alt="Image 3"
            class="imagem-banner"
          ></b-img>
        </b-col>
        <b-col>
          <b-img
            fluid
            src="../css/images/foto4.jpg"
            alt="Image 3"
            class="imagem-banner"
          ></b-img>
        </b-col>
      </b-row>
      <b-row>
        <b-col>
          <b-img
            fluid
            src="../css/images/foto2.jpg"
            alt="Image 3"
            class="imagem-banner"
          ></b-img>
        </b-col>
        <b-col>
          <b-img
            fluid
            src="../css/images/foto3.jpg"
            alt="Image 3"
            class="imagem-banner"
          ></b-img>
        </b-col>
        <b-col>
          <b-img
            fluid
            src="../css/images/foto4.jpg"
            alt="Image 3"
            class="imagem-banner"
          ></b-img>
        </b-col>
        <b-col>
          <b-img
            fluid
            src="../css/images/foto3.jpg"
            alt="Image 3"
            class="imagem-banner"
          ></b-img>
        </b-col>
      </b-row>
    </b-container>

    <!-- <h1 class="title">Rayssa e Jeremias</h1> -->
    <img class="title" src="../css/images/logo_header.png" alt="" />
  </div>
</template>

<script>
export default {};
</script>

<style>
.imagem-banner {
  object-fit: cover;
  height: 100%;
}

.banner-wrapper {
  align-items: center;
  /* border: 1px solid red; */
  height: 100vh;
  width: 100vw;
  overflow: hidden;
  /* display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: repeat(3, 1fr); */

  padding: 0 !important;
  opacity: 0.6;
}

.col {
  padding: 0;
}

.wrapper-banner {
  position: relative;
}

.title {
  position: absolute;
  top: 50%;
  left: 50%;
  z-index: 999;
  transform: translate(-50%, -50%);
  color: rgb(78, 2, 78);
  font-weight: 800;
  font-family: Cambria, Cochin, Georgia, Times, "Times New Roman", serif;
  opacity: 1;
  width: 200px;
}

@media screen and (max-width: 600px) {
}
</style>
