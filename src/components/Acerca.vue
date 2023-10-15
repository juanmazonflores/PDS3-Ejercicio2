<template>
    <section id="acerca">
        <h1>Acerca de mi</h1>

        <div class="acerca-container fx-row fx-column-responsive fx-content-space-between fx-align-items-center">

            <div class="acerca-info fx-column">
                <div class="acerca-contenido fx-row">
                    <div class="acerca-icono">
                        <img src="../assets/iconos/info.png" alt="Info">
                    </div>
                    <div class="acerca-texto">
                        <h3>Información</h3>
                        <div class="acerca-item">
                            <h4>// Nombre:</h4>
                            <p>* Juan Manuel Mazon Flores</p>
                        </div>
                        <div class="acerca-item">
                            <h4>// Información academica:</h4>
                            <p>* Estudiante de 9o semestre Ingenieria en Sistemas de Información - Universidad de
                                Sonora</p>
                        </div>
                        <div class="acerca-item">
                            <h4>// Intereses:</h4>
                            <p>* Backend y Frontend</p>
                        </div>
                        <div class="acerca-item">
                            <h4>// Pasatiempos:</h4>
                            <p>* Videojuegos y Musica</p>
                        </div>
                    </div>
                </div>
            </div>
            <div class="acerca-video fx-column fx-align-items-center fx-content-center">
                <h3>Biografía</h3>
                <iframe src="https://drive.google.com/file/d/1InnYM_M-dTvlrNRYMlNVH23jdeEo0KsE/preview" width="640"
                    height="480" allow="autoplay"></iframe>
                <p>Video biografico</p>
            </div>
        </div>
    </section>
</template>

<script>

export default {
  name: 'Acerca',
}

</script>

<style>

/* ACERCA DE MI */
.acerca-container {
  padding: 0 90px;
  gap: 90px;
}

.acerca-video {
  flex: 1;
  text-align: center;
  padding: 2rem;
  color: var(--color-font);
  background: var(--color-container);
  box-shadow: 0 10px 8px rgba(95, 186, 167, 0.1);
}

.acerca-video iframe{
  width: auto;
  margin-top: 1rem;
 }

.acerca-video h3,
.acerca-video p {
  margin-top: 1rem;
}


.acerca {
  flex: 1;
  gap: 20px;
}

.acerca-item{
  margin-top: 1.5rem;
}

.acerca-contenido {
  gap: 10px;
  padding: 15px;
}

.acerca-icono img {
  width: 40px;
  border-radius: 50%;
}

.acerca-texto {
  flex: 1;
  color: var(--color-font2);
  line-height: 150%;
  
}
</style>
