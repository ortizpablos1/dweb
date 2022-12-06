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
          <h3>Material de Apoyo dedicado al Diseño y Desarrollo Web.</h3>
          <h4>Temas</h4>
          <section class="icontem">
            <div class="conticons">
              <router-link to="/"><img class="iconos" src="@/assets/img/htmlicon2.svg" alt="HTML"></router-link>
            </div>
            <div class="conticons">
              <router-link to="/"><img class="iconos" src="@/assets/img/cssicon2.svg" alt="CSS"></router-link>
            </div>
            <div class="conticons">
              <router-link to="/"><img class="iconos" src="@/assets/img/jsicon2.svg" alt="Js"></router-link>
            </div>
            <div class="conticons">
              <router-link to="/directivas"><img class="iconos" src="@/assets/img/vueicon2.svg" alt="VueJs"></router-link>
            </div>
           
          </section>
          <!-- <button class="btnexplorar" type="submit" ><router-link to="/about"></router-link>Explorar</button>
          <router-link to="/about" class="btnexplorar" data-bs-toggle="modal" data-bs-target="#staticBackdrop">Explorar</router-link>
           -->
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
  font-size: 15px;
  border-radius: 5px;
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
  margin-top: 5px;
  border-radius: 0;
  font-size: 40px;
  background-color: #39A900;
  padding: 8px;
  text-decoration: none;
  color: black;
  border-radius: 5px;
  
}
.btnexplorar:hover{
  color: white;
  background-color: #82DEF0;
  padding: 15px;
}
.icontem{
  margin-top: 5px;
  border: 2px solid rgba(153, 152, 152, 0.253);
  border-radius: 5px;
  display: flex;
}
.conticons{
  width: 100%;
}
.iconos{
  max-width: 100%;
  width: 90%;
  margin: 5px;
}
.iconos:hover{
  border-radius: 100px;
  box-shadow: 0px 0px 20px black;
  width: 85%;
}
 footer{
  height: 5vh;
  display: flex;
  justify-content: flex-end;
  align-items: center;
  color:#00324D;
 }
</style>
