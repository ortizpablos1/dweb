<template>
  <div class="home">
    <header>
      <a href="#"><img class="logo" src="@/assets/img/logo.svg" alt="Logo"></a>
      <nav>
        <ul class="menu">
          <li>Inicio</li>
          <li>Nosotros</li>
          <li>Conctacto</li>
          <li class="ingreso"><b>Entrar</b></li>
        </ul>
      </nav>
    </header>
    <main>
      <section class="principal">
        <artcle class="titulo">
          <h1>Desarrollo Web</h1>
          <h3>Material de didactico dedicado al Diseño y Desarrollo Web.</h3>
          
          <!-- <button class="btnexplorar" type="submit" ><router-link to="/about"></router-link>Explorar</button> -->
          <router-link to="/about" class="btnexplorar">Explorar</router-link>
        </artcle>
        <artcle class="temas">
          <img class="temaimg" src="@/assets/img/tema.svg" alt="Tema">
        </artcle>
      </section>
    </main>
    <footer>
      <b>Instructor: Pablo Ortiz G.</b>
    </footer>
    <TemasCompoment/>
    
  </div>
</template>

<script>
// @ is an alias to /src

import TemasCompoment from '@/components/TemasCompoment.vue';


export default {
  name: 'HomeView',
  components: {
    TemasCompoment
}
}
</script>
<style scoped>
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
 .home{
    background-image: url('@/assets/img/background.svg');
    background-size: cover; 
 }
 header{
  padding-top: 10px;
  height: 10vh;
  display: flex;
  justify-content: space-between;
  align-items: center;
 }
 nav{
  width: 40%;
  height: 30px;
 }
 .menu{
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  
}
li{
  list-style: none;
}
.logo{
  width: 20%;
}
 main{
  height: 85vh;
 }
.ingreso{
  background-color: #39A900;
  padding: 10px;
  font-size: 20px;
} 
.ingreso:hover{
 color: white;
 background-color: #82DEF0;
padding: 15px;
 
}
 
.principal{
  display: flex;
  justify-content: space-around;
  align-items: center;
}
.titulo{
  width: 40%;
  font-size: 40px;
  font-family: Calibri, sans-serif;
  padding: 1%;
  margin-left: 10px;
  
}
h1{
  font-size: 75px;
}
h3{
  font-size: 40px;
  margin-bottom: 40px;
}
.temas{
  width: 60%;
  padding: 1%;
  
}
.temaimg{
  width: 72%;
  
}
.btnexplorar{
  border:0;
  margin-top: 120px;
  border-radius: 0;
  font-size: 40px;
  background-color: #39A900;
  padding: 8px;
  text-decoration: none;
  color: black
  
}
.btnexplorar:hover{
  color: white;
  background-color: #82DEF0;
  padding: 15px;
}
 footer{
  height: 5vh;
  display: flex;
  justify-content: flex-end;
  align-items: center;
  color:#00324D;
 }
</style>
