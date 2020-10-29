<template>
<div id="app">
    <header>
      <Logo></Logo>
      <Navmovil></Navmovil>
    <Nav></Nav>
    </header>
    <main>
      <Banner></Banner>
      <Descripcion></Descripcion>
      <Cards></Cards>
      <Cards></Cards>
      <Registro></Registro>
      <Fotos></Fotos>
      <Album></Album>
      <Footer></Footer>
    </main>
  </div>
</template>

<script>
import Nav from './components/Nav'
import Navmovil from './components/Navmovil'
import Logo from './components/Logo'
import Banner from './components/Banner'
import Descripcion from './components/Descripcion'
import Cards from './components/Cards'
import Registro from './components/Registro'
import Fotos from './components/Fotos'
import Album from './components/Album'
import Footer from './components/Footer'

export default {
  name: 'app',
  components: {
    Nav,
    Navmovil,
    Logo,
    Banner,
    Descripcion,
    Cards,
    Registro,
    Fotos,
    Album,
    Footer
  }
}
</script>

<style>
:root {
    --bckg: white;
    --color-secundario: #912c44;
    --color-nav: #FFE5EB;
    --rgba-hover-nav: rgba(255,255,255,.6);
    --color-submenu: rgba(255,229,235,0.7) ;
    --color-fuente-nav: black;
    --color-fuente-logo-titulo: black;
    --color-fuente-logo-contenido: black;
    --color-fuente-hover-nav: #912c44;
    --gradientbanner: rgba(255, 255, 255, 0.6);
    --bckgreg: #E5EAF0;
    --bckglog: #ffffff;
    --color-button-reg: #ff668a;
    --color-border-reg: #949494;

    /**Fuentes/ */
    --font-titulo: 'Satisfy', cursive;
    --font-subtitulo: 'Special Elite', cursive;
    --font-content: 'Titillium Web', sans-serif;
}
body {
  margin: 0;
}
.text-center {
  text-align: center;
}



</style>
