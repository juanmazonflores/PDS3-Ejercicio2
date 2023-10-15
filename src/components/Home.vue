<template>
    <section id="home" class="scene">
    <div class="home-banner fx-row fx-column-responsive fx-align-items-center fx">
        <div class="home-descripcion">
            <h1>Juan Mazon</h1>
            <h3>Bienvenido a mi sitio</h3>
            <p>Hola, soy Juan Mazon, estudiante de 9no semestre de Ingenieria en Sistemas de Informacion,
                apasionado por la programacion, con especial interes por el desarrollo web, mis hobbies
                son los videojuegos y escuchar musica.
            </p>
        </div>
        <img src="../assets/variedad/mifoto.jpg" alt="Juan Mazon" class="pfp">

        <img src="../assets/fondos/forest.png" class="forest">
    </div>
</section>

</template>

<script>

export default {
  name: 'Home',
  data() {
    return {
      image: "../assets/variedad/mifoto.jpg",
      text: "Juan Mazon"
    }
  }
}
</script>

<style>

/*HEADER*/
#home {
  height: 100vh;
  background-size: cover;
  color: var(--color-font);
  background: url("../assets/fondos/home3.gif") no-repeat center center fixed;
  background-size: cover;
}

.home-banner {
  opacity: 0.9;
  padding: 7rem 10rem;
  z-index: 1;
}

.home-banner > h1 {
  text-transform: uppercase;
  font-size: 2rem;
  width: 100px;
  height: 100px;
}

.home-banner > h3 {
  font-size: 1.5rem;
}

.home-banner > p {
  width: 5rem;
}

.home-descripcion{
  margin-bottom: 5rem;
  margin-right: 5rem;
}

.scene{
  position:relative;
  width: 100%;
  height: 100vh;
  background: linear-gradient(#111425,#3751e0);
  background-attachment: fixed;
  overflow: hidden;
}

.forest{
  position:absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  z-index:1000;
  transform: scale(1.2);
}

.pfp{
  position: relative;
  width: 30%;
  z-index:1;
}

</style>

