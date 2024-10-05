<script setup>
// Importar desde la carpeta `components`
import { datosPersona } from './components/datos';
import  banderaImg from './assets/chile_bandera.png';
import  fotoImg  from './assets/foto_elon.jpg';

const {
  run,
  apellidos,
  nombres,
  nacionalidad,
  sexo,
  fechaDeNacimiento,
  numeroDeDocumento,
  fechaDeEmision,
  fechaDeVencimiento,
  firmaTitular
} = datosPersona;

</script>

<template>
  <div class="carnet" data-aos="flip-right" data-aos-delay="500">
    <aside>
      <div>
        <span>CEDULA DE INDENTIDAD</span>
        <img width="40" :src="banderaImg" alt="" />
      </div>

      <img :src="fotoImg" alt="" />
      <p>RUN {{ run }} </p>
    </aside>

    <main>
      <header>
        <p>REPUBLICA DE CHILE</p>
        <span>SERVICIO DE REGISTRO CIVIL E IDENTIFICACIÓN</span>
      </header>
      <section>
        <article>
          <header>APELLIDOS</header>
          <span>{{ apellidos }}</span>
        </article>
        <article>
          <header>NOMBRES</header>
          <span>{{ nombres }}</span>
        </article>

        <div class="grid-2-colums">
          <article>
            <header>NACIONALIDAD</header>
            <span>{{ nacionalidad }}</span>
          </article>
          <article>
            <header>SEXO</header>
            <span> {{ sexo }}</span>
          </article>
        </div>
        <div class="grid-2-colums">
          <article>
            <header>FECHA DE NACIMIENTO</header>
            <span>{{ fechaDeNacimiento }}</span>
          </article>
          <article>
            <header>NÙMERO DOCUMENTO</header>
            <span>{{ numeroDeDocumento }}</span>
          </article>
        </div>
        <div class="grid-2-colums">
          <article>
            <header>FECHA DE EMISIÒN</header>
            <span>{{ fechaDeEmisión }}</span>
          </article>
          <article>
            <header>FECHA DE VENCIMIENTO</header>
            <span>{{ fechaDeVencimiento }}</span>
          </article>
        </div>
        <article>
          <header>FIRMA DEL TITULAR</header>
          <span>{{ firmaTitular }}</span>
        </article>
      </section>
    </main>
  </div>
</template>

<style scoped>
body {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 60vh;
  font-size: 10px;
  font-family: sans-serif;
}

.carnet {
  width: 400px;
  height: 240px;
  background: #c8deed;
  border-radius: 20px;
  display: grid;
  grid-template-columns: 30% 1fr;
  padding: 15px;
  box-shadow: 0px 0px 10px 2px black;
}

aside div {
  display: flex;
}

aside>img {
  margin-top: 15px;
  width: 100%;
}

aside p {
  text-align: center;
  font-size: 12px;
  font-weight: bold;
}

main {
  padding: 0px 20px;
}

main article {
  margin: 4px 0px;
}

main article header {
  font-weight: bold;
  color: #0235a4;
  font-size: 8px;
}

main header p {
  font-size: 20px;
  margin: 0;
  font-weight: bold;
  color: #0235a4;
}

main header span {
  font-size: 8px;
  color: #399be1;
}

main section {
  margin-top: 10px;
}

main section article span {
  font-size: 13px;
  font-weight: 600;
}

main section .grid-2-colums {
  display: grid;
  grid-template-columns: 50% 50%;
}
</style>