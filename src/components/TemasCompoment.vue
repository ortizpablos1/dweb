<template>
<div class="modal" id="staticBackdrop" data-bs-backdrop="static" data-bs-keyboard="false" tabindex="-1" aria-labelledby="staticBackdropLabel" aria-hidden="true">
  <div class="modal-dialog">
    <div class="modal-content">
      <div class="modal-header">
        <h1 class="modal-title fs-5" id="staticBackdropLabel">Tematicas</h1>
        <!-- <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button> -->
      </div>
      <section class="cards">
        <article class="card">
          <router-link to="/directivas"><img src="@/assets/img/logo.png" alt="Vue" data-bs-dismiss="modal"></router-link>
          <h2>Vue Js</h2>
        </article>
        <article class="card">
          <router-link to="/directivas"><img src="@/assets/img/logo.png" alt="Vue" data-bs-dismiss="modal"></router-link>
          <h2>Vue Js</h2>
        </article>
        <article class="card">
          <router-link to="/directivas"><img src="@/assets/img/logo.png" alt="Vue" data-bs-dismiss="modal"></router-link>
          <h2>Vue Js</h2>
        </article>
        <article class="card">
            <img src="@/assets/img/logo.png" alt="Vue">
            <h2>HTML</h2>
        </article>
        <article class="card">
            <img src="@/assets/img/logo.png" alt="Vue">
            <h2>CSS</h2>
      </article>
    </section>  
      <div class="modal-footer">
        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Cerrar</button>
      </div>
    </div>
  </div>
</div>


</template>
<script>
export default {
    name: 'TemasComponent',
    setup(){

    }
}
</script>
<style scoped>
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
    .cards{
        display: flex;
        flex-wrap: wrap;
        justify-content: space-evenly;
        align-items: center;
        width: 90%;
        margin: auto;
    }
    .card{
        border: 1px solid grey;
        width: 20%;
        height: 20%;
        border-radius: 3px;
    }
    .modal-content{
      
      width: 120%;
      margin: auto;
    }
    
</style>

