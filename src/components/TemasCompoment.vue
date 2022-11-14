<template>
    <section class="cards">
        <article class="card">
            <img src="@/assets/img/logo.png" alt="Vue">
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
        width: 80%;
        margin: auto;

    }
    .card{
        border: 1px solid grey;
        width: 20%;
        height: 20%;
        border-radius: 3px;
    }
</style>

