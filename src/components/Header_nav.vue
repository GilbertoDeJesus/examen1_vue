<script>
export default {
    props: {
        url: {
            String
        },
        nombreEmpresa: {
            String
        },
        nombreAlumno: {
            String
        },
        grupo: {
            String
        },
    },

};
</script>

<template>
    <div>
        <div class="fixed-top bg-primary px-4 text-white text-center"><p>{{nombreEmpresa}}<strong> | Telefono para pedidos: 952 03 99 50</strong></p></div>
        <nav class="navbar navbar-expand-lg fixed-top navbar-light bg-light pl-8 pr-8 mt-4">
            <a class="navbar-brand" href="#">
                <img v-bind:src="url" width="40" height="40" alt="Logo"> {{nombreEmpresa}}
            </a>
            <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent"
                aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>

            <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <span class="text-dark pr-4">{{nombreAlumno}} <strong>{{grupo}}</strong></span>
                <ul class="navbar-nav nav-pills mr-auto">
                    <li class="nav-item mr-4 mb-1">
                        <a class="nav-link active text-white" href="#">ENSALADAS</a>
                    </li>
                    <li class="nav-item mr-4 mb-1">
                        <a class="nav-link active text-white" href="#">ARROCES</a>
                    </li>
                    <li class="nav-item mr-4 mb-1">
                        <a class="nav-link active text-white" href="#">PESCADOS</a>
                    </li>
                    <li class="nav-item mr-4 mb-1">
                        <a class="nav-link active text-white" href="#">CARNES</a>
                    </li>
                    <li class="nav-item mr-4 mb-1">
                        <a class="nav-link active text-white" href="#">POSTRES</a>
                    </li>
                </ul>
                <span class="navbar-text">
                    <strong><svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor"
                            class="bi bi-cart4" viewBox="0 0 16 16">
                            <path
                                d="M0 2.5A.5.5 0 0 1 .5 2H2a.5.5 0 0 1 .485.379L2.89 4H14.5a.5.5 0 0 1 .485.621l-1.5 6A.5.5 0 0 1 13 11H4a.5.5 0 0 1-.485-.379L1.61 3H.5a.5.5 0 0 1-.5-.5zM3.14 5l.5 2H5V5H3.14zM6 5v2h2V5H6zm3 0v2h2V5H9zm3 0v2h1.36l.5-2H12zm1.11 3H12v2h.61l.5-2zM11 8H9v2h2V8zM8 8H6v2h2V8zM5 8H3.89l.5 2H5V8zm0 5a1 1 0 1 0 0 2 1 1 0 0 0 0-2zm-2 1a2 2 0 1 1 4 0 2 2 0 0 1-4 0zm9-1a1 1 0 1 0 0 2 1 1 0 0 0 0-2zm-2 1a2 2 0 1 1 4 0 2 2 0 0 1-4 0z" />
                        </svg> $0.00</strong>
                </span>
            </div>
        </nav>
    </div>
</template>

<style scoped>

</style>