<template>
    <div id="app">
        <div class="contenedor" v-for="(personaje, index) in personajes" :key="index">
            <img class="img" :src="personaje.src" alt="">
            <h3 class="nombre">{{personaje.nombre}}</h3>
        </div>
    </div>
</template>

<script>
export default {
    name: "RickAndMorty",
    data: () => ({
        personajes:[
        {
            nombre: "Rick Sanchez",
            src: "https://rickandmortyapi.com/api/character/avatar/1.jpeg"
        },
        {
            nombre: "Morty Smith",
            src: "https://rickandmortyapi.com/api/character/avatar/2.jpeg"
        },
        {
            nombre: "Summer Smith",
            src: "https://rickandmortyapi.com/api/character/avatar/3.jpeg"
        },
        {
            nombre: "Berth Smith",
            src: "https://rickandmortyapi.com/api/character/avatar/4.jpeg"
        },
        {
            nombre: "Jerry Smith",
            src: "https://rickandmortyapi.com/api/character/avatar/5.jpeg"
        }]
    })
}   
</script>

<style scoped>
#app {
  background-image: url("https://rickandmortypod.com/wp-content/uploads/2018/11/cropped-RM_page-header_background1-3.png");
  background-size: cover;
}

.contenedor {
    display: flex;
    flex-direction: row;
    align-items: center;
}

.img {
    width: 200px;
    border-radius: 50%;
    padding: 2rem;
}
.nombre {
    color: green;
    font-size: 2rem;
}
</style>