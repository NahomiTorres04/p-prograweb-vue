<template>
    <nav>
        <ul>
            <li><a href="#">Nosotros</a></li>
            <li><a href="#">Productos</a></li>
            <li class="submenu">
                <a href="#">Categorias<i class="fas fa-caret-down"></i></a>
                <ul class="children">
                    <li><a href="#">SubElemento #1</a></li>
                    <li><a href="#">SubElemento #2</a></li>
                    <li><a href="#">SubElemento #3</a></li>
                </ul>
            </li>
            <h1>NT</h1>
            <li><a href="#">Inicia Sesión</a></li>
            <li class="submenu">
                <a href="#">Catalogos<i class="fas fa-caret-down"></i></a>
                <ul class="children">
                    <li><a href="#">SubElemento #1</a></li>
                    <li><a href="#">SubElemento #2</a></li>
                    <li><a href="#">SubElemento #3</a></li>
                    <li><a href="#">SubElemento #2</a></li>
                    <li><a href="#">SubElemento #3</a></li>
                </ul>
            </li>
            <li><a href="#">Contacto</a></li>
        </ul>
    </nav>
</template>

<script>
export default {
    name: "Nav",
}
</script>

<style scoped>
nav {
  width: 100%;
  height: 60px;
  z-index: 1000;
  background: var(--color-nav);
  display: flex;
  justify-content: center;
  align-items: center;
}
nav ul {
  width: 100%;
  height: 95%;
  padding: 0;
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
  align-items: center;
}
nav ul li {
  list-style: none;
  position: relative;
  display: inline-block;
}
nav ul h1{
    font-family: var(--font-titulo);
    font-size: 45px;
    color: var(--color-fuente-hover-nav);
}
nav ul li:hover {
  background: var(--rgba-hover-nav);
}
nav ul li:hover a {
  color: var(--color-fuente-hover-nav);
}
nav ul img {
  height: 90%;
}
nav ul li a {
  padding: 15px;
  display: block;
  text-decoration: none;
  color: var(--color-fuente-nav);
  font-family: var(--font-content);
  font-size: 17px;
}
nav ul li a i {
  margin-left: 10px;
}

nav ul li:hover .children {
  display: block;
}
nav ul li .children {
  display: none;
  background: var(--color-submenu);
  position: absolute;
  width: 200%;
  padding: 15px;
  height: auto;
  width: 160%;
  z-index: 1000;
}
@media screen and (max-width: 700px) {
  nav {
    width: 80%;
    height: calc(100% - 80px);
    position: fixed;
    right: 100%;
    margin: 0;
    overflow: scroll;
    background: black;
  }
  nav ul {
    width: 95%;
    flex-direction: column;
    position: absolute;
  }
  nav ul li {
    width: 95%;
    text-align: left;
    display: block;
    border-bottom: solid 1px #24fb7b;
  }
  nav ul li a {
    padding: 20px 15px;
    display: block;
    color: #24fb7b;
    font-size: 30px;
    text-align: left;
  }
  nav ul li .children {
    width: 100%;
    position: relative;
  }
  nav ul img {
    display: none;
  }
  nav ul li:hover .children {
    display: none;
  }
}

</style>