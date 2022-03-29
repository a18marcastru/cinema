<template>
    <br>
    <h1>Cartella</h1>
    <div id="container">
    <div v-for="sess in sessiones">
        <p>{{sess.titulo}}</p>
        <img :src="sess.poster"/>
    </div>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                sessiones: [
                    {
                        id_session: "1",
                        dias: ["Lunes","Martes","Miercoles"],
                        horas: ["10:00","12:30","15:00","18:30","21:00"],
                        butacas: [1,2,3,4,5,6,7,8,9,10],
                        precio: "10€",
                        dia_espectador: "Nerd",
                        titulo: "Shrek",
                        descripcion: "Ogro que habla con un burro.",
                        poster: "https://m.media-amazon.com/images/M/MV5BOGZhM2FhNTItODAzNi00YjA0LWEyN2UtNjJlYWQzYzU1MDg5L2ltYWdlL2ltYWdlXkEyXkFqcGdeQXVyMTQxNzMzNDI@._V1_SX300.jpg",
                        anyo: "2001"
                    },
                    {
                        id_session: "2",
                        dias: ["Martes","Jueves","Viernes"],
                        horas: ["10:00","12:30","15:00","18:30","21:00"],
                        butacas: [1,2,3,4,5,6,7,8,9,10],
                        precio: "10€",
                        dia_espectador: "Nerd",
                        titulo: "Cars",
                        descripcion: "Un coche que quiere ser el mejor.",
                        poster: "https://m.media-amazon.com/images/M/MV5BMTg5NzY0MzA2MV5BMl5BanBnXkFtZTYwNDc3NTc2._V1_SX300.jpg",
                        anyo: "2006"
                    }
                ],
                User: [
                    {
                        "id_user": "1",
                        "nombre": "Marc",
                        "apellido": "Castro",
                        "correo": "marc@gmail.com",
                        "contrasenya": "Marcfv1302*?*"
                    }
                ]
            }
        },
        components: {
        },
        methods: {
        },
    }
</script>

<style>
    #container {
        display: grid;
        grid-template-columns: auto auto;
    }
</style>