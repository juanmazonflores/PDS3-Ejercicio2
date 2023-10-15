<template>
    <footer id="footer" class="fx-column fx-content-center fx-align-items-center">

        <div class="contacto-container">

        <h2>Contacto</h2>

        <form id="contacto-form" class="fx-column">

            <input type="text" id="nombre" placeholder="Nombre" required>

            <input type="email" id="email" placeholder="Email" required>

            <textarea id="mensaje" placeholder="Mensaje" required></textarea>

            <button type="submit" class="button-action">Enviar</button>

        </form>

        </div>

        <div class="redes-sociales-container fx-row">

        <a href="https://github.com/juanmazonflores" target="_blank"><i class="fa-brands fa-github"></i></a>
        <a href="https://www.facebook.com/juanmanuel.masonflores" target="_blank"><i class="fa-brands fa-facebook"></i></a>
        <a href="https://twitter.com/juanitomaflo" target="_blank"><i class="fa-brands fa-x-twitter"></i></a>
        <a href="https://www.linkedin.com/in/juan-mazon-653472277/" target="_blank"><i class="fa-brands fa-linkedin"></i></a>

        </div>

        <p>Juan Manuel Mazon Flores &copy; 2023</p>

    </footer>
</template>

<script>
    export default {
      name: 'Footer',
    }

    document.addEventListener("DOMContentLoaded", () => {

    const contactoForm = document.getElementById('contacto-form');

  contactoForm.addEventListener("submit", (event) => {
    event.preventDefault();

    const nombre = document.getElementById("nombre").value;
    const email = document.getElementById("email").value;
    const mensaje = document.getElementById("mensaje").value;

    alert('Gracias por contactarnos - Nombre: ' + nombre + '- Email: ' + email + '- Mensaje: ' + mensaje);

    contactoForm.reset();
  });

});
</script>

<style>
footer {
  color: var(--color-font2);
  text-align: center;
  padding: 6rem 3rem;
}

.contacto-container{
  width: 600px;
  max-width: 100%;

}

.contacto-container h2 {
  font-size: 2rem;
  margin-bottom: 2rem;

}

input,
textarea {
  margin-bottom: 1rem;
  padding: 8px;
  background-color: var(--color-container);
  font-family: var(--font-family);
  font-weight: 400;
  opacity: 0.8;
  color: var(--color-font);
  font-size: 20px;
}

input::placeholder,
textarea::placeholder{
  color: var(--color-font);
  font-size: 20px;
  opacity: 0.8;
}

.redes-sociales-container {
  gap: 1.5rem;
  margin-top: 2rem;
  margin-bottom: 2rem;
  padding: 0.5rem;
  opacity: 0.6;
  background-color: var(--color-background);
}

.fa-brands {
  font-size: 2rem;
  color: var(--color-button2);
}

.fa-brands:hover {
  background-color: var(--color-button);
}

.fa-brands:active {
  color: var(--color-button);
}


/*RESPONSIVE*/
@media screen and (max-width: 1125px) {
  .fx-column-responsive{
    display: flex;
    flex-direction: column;
  }

  button.button-action{
    font-size: 1rem;
  }
  .home-banner {
    opacity: 0.9;
    padding: 15rem 10rem;
    z-index: 1;
  }
  .header-content{
    padding: 30px;
    margin-top:100px
  }

  .home-banner {
    opacity: 0.9;
    padding: 7rem 10rem;
    z-index: 1;
  }

  .home-descripcion{
    margin-bottom: 0rem;
    margin-right: 0rem;
  }

  .pfp{
    position: relative;
    width: 50%;
    z-index: 1;
    margin-top: 5%;
  }
  .home-banner{
    text-align: center;
  }
  .modal > div {
    width: 400px;
    top: 50px;
  }

}

@media screen and (max-width: 768px) {
 

  .menu{
    padding: 20px;
    justify-content: space-between;
    display: flex;
    flex-direction: column;
  } 
  .menu label{
    display: initial;
  }
  .menu .navbar{
      position:absolute;
      top:100%;
      left:0;
      right: 0;
      background-color: var(--color-background);
      height: auto;
      display: none;
      opacity: 1;
  }
  .menu .navbar ul li{
      width: 100%;
  }

  #menu:checked ~ .navbar{
      display: initial;
  }

  section {
    padding: 40px 45px;
  }

  section > h1 {
    text-align: center;
    margin-left: 0rem;
  }


  
}
</style>