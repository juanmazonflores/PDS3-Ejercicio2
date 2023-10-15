<template>
    <header id=¨header¨ class="fx-row fx-content-space-between fx-align-items-center">
        <div class="menu container">
            <input type="checkbox" id="menu" />
            <label for="menu">
                <img src="../assets/iconos/menu.png" class="menu-icono">
            </label>
            <nav class="navbar">
                <ul class="fx-row fx-align-items-center fx-content-space-between">
                    <li><a href="#acerca">Acerca de mi</a></li>
                    <li><a href="#habilidades">Habilidades</a></li>
                    <li><a href="#proyectos">Proyectos Destacados</a></li>
                </ul>

            </nav>
        </div>

        <a id="logo">
            <img src="../assets/variedad/logo.png" title="Juan Mazon">
        </a>


        <a id="contacto" href="#footer">
            <i class=" fx-content-space-between fa-solid fa-phone" title="Contacto"></i>
        </a>
    </header>
</template>

<script>
    export default {
      name: 'Navbar',
    }
    
</script>

<style>

#menu{
  display: none;
}

.menu-icono{
  width: 25px;
}

.menu label{
  cursor: pointer;
  display: none;
}

header {
  position: fixed;
  width: 100%;
  height: 90px;
  background-color: #000000;
  opacity: 0.9;
  box-shadow: 0 6px 8px rgba(0, 0, 0, 0.10);
  z-index: 1;
}

#contacto {
  margin: 10px;
  width: auto;
  padding: 5px;
}

#logo img{
  width: 275px;
  cursor: pointer;
  padding: 5px;
}

nav {
  height: 50px;
  font-size: 1.25rem;
}
nav ul {
  list-style: none;
  margin-bottom: 0;
}
nav li {
  padding: 0.75rem 2rem;
  font-weight: 300;
}

nav a {
  text-decoration: none;
  color: var(--color-font2);
}

nav ul li:hover{
  color: var(--color-background);
  cursor: pointer;
  background-color: var(--color-button);
}

.fa-solid,.fa-brands {
  font-size: 2rem;
  color: var(--color-font2);
  padding: 0.5rem;
}

.fa-solid:hover,.fa-brands:hover {
  background-color: var(--color-button);
}

</style>