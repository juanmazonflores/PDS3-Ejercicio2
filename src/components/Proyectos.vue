<template>

    <section id="proyectos">
        <h1>Proyectos Destacados</h1>
        <div class="card-container fx-row fx-column-responsive fx-content-space-between">

            <div class="card fx-column">
                <div class="card-imagen">
                    <img src="../assets/proyectos/play1.png" alt="Proyecto 1">
                </div>
                
                <h3>Play&Star</h3>
                <p>Descripción: Sistema web para mantenerte informado sobre las ultimas noticias del cine, 
                    incluye peliculas destacadas, director destacado, reconocimientos proximos y mapa de ubicacion
                </p>
                <button onclick="location.href='#openModal1'" class="button-action">Ver Detalle</button>
                <div id="openModal1" class="modal">
                    <div>
                        <a href="#close" title="Close" class="close">X</a>
                        <div class="fx-column">
                            <h2>Play&Star</h2>
                            <div class="slider-container2">
                                <div class="slider-item">
                                    <img src="../assets/proyectos/play2.png" alt="Imagen 1">
                                    <p>Seccion de Peliculas Destacadas con un Swiper</p>
                                </div>
                                <div class="slider-item">
                                    <img src="../assets/proyectos/play3.png" alt="Imagen 1">
                                    <p>Seccion de Director Destacado</p>
                                </div>
                                <div class="slider-item">
                                    <img src="../assets/proyectos/play4.png" alt="Imagen 1">
                                    <p>El proyecto incluye una seccion de Contacto </p>
                                </div>
                            </div>  
                        </div>
                    </div>
                </div>
            </div>

            <div class="card fx-column">
                <div class="card-imagen">
                    <img src="../assets/proyectos/jungle1.png" alt="Proyecto 2">
                </div>
                
                <h3>Jungle-Jump</h3>
                <p>Videojuego cuyo objetivo principal es esquivar objetos de manera horizontal
                    generados aleatoriamente, permite pausar, detener y reiniciar.</p>
                <button onclick="location.href='#openModal2'" class="button-action">Ver Detalle</button>
                <div id="openModal2" class="modal">
                    <div>
                        <a href="#close" title="Close" class="close">X</a>
                        <div class="fx-column fx-align-items-center">
                            <h2>Jungle-Jump</h2>

                            <div class="slider-container2">
                                <div class="slider-item">
                                    <img src="../assets/proyectos/jungle2.png" alt="Imagen 1">
                                    <p>El personaje puede saltar para esquivar enemigos</p>
                                </div>
                                <div class="slider-item">
                                    <img src="../assets/proyectos/jungle3.png" alt="Imagen 1">
                                    <p>Se gana al llegar a la meta</p>
                                </div>
                                <div class="slider-item">
                                    <img src="../assets/proyectos/jungle4.png" alt="Imagen 1">
                                    <p>Si un enemigo te toca, pierdes</p>    
                                </div>
                            </div>   
                        </div>
                    </div>
                </div>

            </div>

            <div class="card fx-column">
                <div class="card-imagen">
                    <img src="../assets/proyectos/ferre1.png" alt="Proyecto 3">
                </div>
                <h3>Ferrefast</h3>
                <p>Aplicación que permite el control de entregas a domicilio en productos de Ferreteria,
                    tanto para vendedores como para clientes</p>
                <button onclick="location.href='#openModal3'" class="button-action">Ver Detalle</button>
                <div id="openModal3" class="modal">
                    <div>
                        <a href="#close" title="Close" class="close">X</a>
                        <div class="fx-column fx-align-items-center">
                            <h2>Ferrefast</h2>
                            <div class="slider-container">

                                <div class="slider-item">
                                    
                                    <img src="../assets/proyectos/ferre2.png" alt="Imagen 1">
                                    <p>Seccion para escoger tus productos</p>
                                </div>
                                <div class="slider-item">
                                    <img src="../assets/proyectos/ferre3.png" alt="Imagen 1">
                                    <p>Detalles de Producto</p>
                                </div>
                                <div class="slider-item">
                                    <img src="../assets/proyectos/ferre4.png" alt="Imagen 1">
                                    <p>Tiene un menu hamburguesa para que el usuario</p>
                                </div>
                            </div>          
                        </div>
                    </div>
                </div>
            </div>


        </div>

    </section>

</template>

<script>
    export default {
        name: 'Proyectos',
    }
</script>

<style>
    
/*PROYECTOS DESTACADOS*/
    .card {
    position: relative;
    overflow: hidden;
    padding: 20px;
    margin: 20px;
    background: var(--color-container);
    text-align: center;
    color: var(--color-font2);
    display: flex;

    }

    .card-imagen{
    height: 100%;
    width: 100%;
    overflow: hidden;
    }

    .card-imagen img {
    height: 100%;
    max-width: 90%;
    }
    .card h3 {
    margin-top: 1rem;
    margin-bottom: 1rem;
    font-size: 1.5rem;
    }
    .card p {
    margin-bottom: 1rem;
    }

    .modal {
        position: fixed;
        font-family: var(--font-family);
        top:0;
        right: 0;
        bottom: 0;
        left: 0;
        background: rgba(0,0,0,0.9);
        z-index: 99999;
        opacity:0;
        -webkit-transition: opacity 400ms ease-in;
        -moz-transition: opacity 400ms ease-in;
        transition: opacity 400ms ease-in;
        pointer-events: none;
    overflow: hidden;
    }
    .modal:target {
        opacity:1;
        pointer-events: auto;
    
    }
    .modal > div {
        width: 500px;
    top: -100px;
        position: relative;
        margin: 10% auto;
        padding: 30px 30px 30px 30px;
        background: var(--color-background2);
    -webkit-transition: opacity 400ms ease-in;
    -moz-transition: opacity 400ms ease-in;
    transition: opacity 400ms ease-in;
    opacity: 0.8;
    
    }


    .modal h2{
    margin-bottom: 1rem;
    }

    .modal img{
    height: 100%;
    width: 100%;
    overflow: hidden;
    }

    .close {
        background: var(--color-background2);
        color: var(--color-font2);
        line-height: 0px;
        position: absolute;
        right: 10px;
        text-align: center;
        width: 24px;
        text-decoration: none;
        font-weight: bold;
    }
    .close:hover { 
    background: var(--color-button2);

    }

    .slider-container {
    display: flex;
    overflow-x: scroll;
    scroll-snap-type: x mandatory;

    }

    .slider-container div {
    flex: 0 0 100%;
    width: 50%;
    height: 50%;
    padding: 20px ;
    object-fit: cover;
    scroll-snap-align: center;

    }

    .slider-container img {
    flex: 0 0 100%;
    width: 70%;
    height: 70%;
    padding: 20px ;
    object-fit: cover;
    scroll-snap-align: center;
    }

    .slider-container2 {
    display: flex;
    overflow-x: scroll;
    scroll-snap-type: x mandatory;

    }

    .slider-container2 div {
    flex: 0 0 100%;
    width: 100%;
    height: 100%;
    padding: 20px ;
    object-fit: cover;
    scroll-snap-align: center;
    }

    .slider-container2 img {
    flex: 0 0 100%;
    width: 100%;
    height: 100%;
    padding: 20px ;
    object-fit: cover;
    scroll-snap-align: center;
    }

    /*MODAL: BARRA SCROLL*/
    .slider-container::-webkit-scrollbar, .slider-container2::-webkit-scrollbar
    {
    width: 12px;
    height: 12px;
    }

    .slider-container::-webkit-scrollbar:window-inactive,
    .slider-container2::-webkit-scrollbar:corner-present  {
    display: none;
    }

    .slider-container::-webkit-scrollbar-track-piece,
    .slider-container2::-webkit-scrollbar-track-piece {
    border-radius: 2px;
    background-color: #369;
    background-clip: content-box;
    border: solid 4px transparent;
    }


    .slider-container::-webkit-scrollbar-button:horizontal:decrement:single-button,
    .slider-container2::-webkit-scrollbar-button:horizontal:decrement:single-button{
    background: transparent url(https://elcssar.com/ejemplos/arrow_left.png) no-repeat center center;
    }

    .slider-container::-webkit-scrollbar-button:horizontal:increment:single-button, 
    .slider-container2::-webkit-scrollbar-button:horizontal:increment:single-button{
    background: transparent url(https://elcssar.com/ejemplos/arrow_right.png) no-repeat center center;
    }

    .slider-container::-webkit-scrollbar-thumb,
    .slider-container2::-webkit-scrollbar-thumb  {
    height: 10px;
    width: 4px;
    background-color: #09C;
    box-shadow: 0 3px 6px -2px rgba(51,0,51,0.5);
    }
    .slider-container::-webkit-scrollbar-corner,
    .slider-container2::-webkit-scrollbar-corner{
    background: transparent ;
    }
    .slider-container::-webkit-resizer,
    .slider-container2::-webkit-resizer {
    background: transparent url(https://elcssar.com/ejemplos/expandIcon.png) no-repeat -1px -1px;
    }

</style>