<template>
    <section id="habilidades">
        <h1>Habilidades</h1>
        <div class="habilidad-container-simbologia fx-row fx-content-center">
            <div class="habilidad-simbologia fx-row fx-content-center">
                <h3>Areas de Experiencia Simbologia:</h3>
            </div>
            <div class="habilidad-simbologia fx-row fx-content-center">
                <img src="../assets/iconos/coding.png" alt="">
                <p>Desarrollo de Sistemas de Escritorio</p>
            </div>
            <div class="habilidad-simbologia fx-row fx-content-center">
                <img src="../assets/iconos/globe.png" alt="">
                <p>Desarrollo Web</p>
            </div>
            <div class="habilidad-simbologia fx-row fx-content-center">
                <img src="../assets/iconos/smartphone.png" alt="">
                <p>Desarrollo Movil</p>
            </div>
        </div>
        <div class="habilidad-container fx-row fx-content-center">
            <div class="habilidad">
                <h3>Lenguajes de Programacion</h3>
                <div class="habilidad-lista fx-column fx-content-center">
                    <div class="habilidad-lista fx-row fx-content-center">
                        <p>Java</p>
                        <img src="../assets/iconos/movil32.png" alt="">
                        <img src="../assets/iconos/escritorio32.png" alt="">

                    </div>
                    <div class="habilidad-lista fx-row fx-content-center">
                        <p>C#</p>
                        <img src="../assets/iconos/escritorio32.png" alt="">

                    </div>
                    <div class="habilidad-lista fx-row fx-content-center">
                        <p>Javascript</p>
                        <img src="../assets/iconos/web32.png" alt="">

                    </div>
                    <div class="habilidad-lista fx-row fx-content-center">
                        <p>Python</p>
                        <img src="../assets/iconos/web32.png" alt="">
                    </div>
                </div>
            </div>
            <div class="habilidad">
                <h3>Bases de Datos</h3>
                <div class="habilidad-lista fx-column fx-content-center">
                    <div class="habilidad-lista fx-row fx-content-center">
                        <p>MySQL</p>
                        <img src="../assets/iconos/web32.png" alt="">
                    </div>
                    <div class="habilidad-lista fx-row fx-content-center">
                        <p>SQL</p>
                        <img src="../assets/iconos/escritorio32.png" alt="">

                    </div>
                </div>
            </div>
            <div class="habilidad">
                <h3>Entornos de Desarrollo</h3>
                <div class="habilidad-lista fx-column fx-content-center">
                    <div class="habilidad-lista fx-row fx-content-center">
                        <p>NetBeans</p>
                        <img src="../assets/iconos/escritorio32.png" alt="">

                    </div>
                    <div class="habilidad-lista fx-row fx-content-center">
                        <p>Visual Studio</p>
                        <img src="../assets/iconos/escritorio32.png" alt="">

                    </div>
                    <div class="habilidad-lista fx-row fx-content-center">
                        <p>Visual Studio Code</p>
                        <img src="../assets/iconos/web32.png" alt="">

                    </div>
                    <div class="habilidad-lista fx-row fx-content-center">
                        <p>Android Studio</p>
                        <img src="../assets/iconos/movil32.png" alt="">

                    </div>
                </div>
            </div>
            <div class="habilidad">
                <h3>Control de Versiones</h3>
                <div class="habilidad-lista fx-column fx-content-center">
                    <div class="habilidad-lista fx-row fx-content-center">
                        <p>Git</p>
                        <img src="../assets/iconos/web32.png" alt="">
                        <img src="../assets/iconos/escritorio32.png" alt="">
                    </div>
                    <div class="habilidad-lista fx-row fx-content-center">
                        <p>Sourcetree</p>
                        <img src="../assets/iconos/web32.png" alt="">

                    </div>
                </div>
            </div>
            <div class="habilidad">
                <h3>Sistemas Operativos</h3>
                <div class="habilidad-lista fx-column fx-content-center">
                    <div class="habilidad-lista fx-row fx-content-center">
                        <p>Windows</p>
                        <img src="../assets/iconos/movil32.png" alt="">
                        <img src="../assets/iconos/web32.png" alt="">
                        <img src="../assets/iconos/escritorio32.png" alt="">

                    </div>
                    <div class="habilidad-lista fx-row fx-content-center">
                        <p>Linux</p>
                        <img src="../assets/iconos/escritorio32.png" alt="">
                    </div>
                </div>
            </div>
            <div class="habilidad">
                <h3>Idiomas</h3>
                <div class="habilidad-lista fx-column fx-content-center">
                    <div class="habilidad-lista fx-row fx-content-center">
                        <p>Español</p>
                        <div class="star-rating">
                            <span class="star">&#9733;</span>
                            <span class="star">&#9733;</span>
                            <span class="star">&#9733;</span>
                            <span class="star">&#9733;</span>
                            <span class="star">&#9733;</span>
                        </div>
                    </div>
                    <div class="habilidad-lista fx-row fx-content-center">
                        <p>Ingles</p>
                        <div class="star-rating">
                            <span class="star">&#9733;</span>
                            <span class="star">&#9733;</span>
                            <span class="star">&#9733;</span>
                            <span class="star">&#9734;</span>
                            <span class="star">&#9734;</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>

    </section>
</template>

<script>
    export default {
        name: 'Habilidades',
    }
</script>

<style>

    /*HABILIDADES*/

    .habilidad-container {
    flex-flow: wrap;
    }

    .habilidad {
    position: relative;
    max-width: 350px;
    overflow: hidden;
    padding: 20px;
    margin: 20px;
    background: var(--color-container2);
    box-shadow: 10px 10px rgba(0, 0, 0, 0.1);
    text-align: center;
    
    }
    .habilidad-lista img {
    margin-left: 1rem;
    margin-bottom: 1rem;
    }


    .habilidad h3 {
    margin-top: 1rem;
    margin-bottom: 1rem;
    font-size: 1.5rem;
    }
    .habilidad p {
    margin-bottom: 1rem;
    margin-top: 0.25rem;
    }

    .habilidad-simbologia{
    position: relative;
    max-width: 350px;
    overflow: hidden;
    padding: 10px;
    margin: 10px;
    color: var(--color-font);
    text-align: center;
    height: 4rem;
    }

    .habilidad-container-simbologia {
    flex-flow: wrap;
    background-color: var(--color-container);
    opacity: 0.8;
    margin: 20px 90px ;
    }

    .habilidad-container-simbologia p { 
    padding-left: 1%;
    }

</style>


