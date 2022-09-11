<template>
    <div class="container is-primary">
        <b-navbar>
        <template #brand>
            <b-navbar-item tag="router-link" :to="{ path: '/' }">
                <img
                    src="https://raw.githubusercontent.com/buefy/buefy/dev/static/img/buefy-logo.png"
                    alt="Lightweight UI components for Vue.js based on Bulma"
                >
            </b-navbar-item>
        </template>
        <template #start>
            <b-navbar-item  tag="router-link" to="/">
                Inicio
            </b-navbar-item>
            <b-navbar-item tag="router-link" to="/about">
                Nosotros
            </b-navbar-item>
            <b-navbar-dropdown label="Almacen">
                <b-navbar-item tag="router-link" to="/categorias">
                    Categorias
                </b-navbar-item>
                <b-navbar-item tag="router-link" to="/medidas">
                    Medidas
                </b-navbar-item>
            </b-navbar-dropdown>
        </template>

        <template #end>
            <b-navbar-item tag="div">
                <div class="buttons">
                    <a class="button is-primary">
                        <strong>Sign up</strong>
                    </a>
                    <a class="button is-light">
                        Log in
                    </a>
                </div>
            </b-navbar-item>
        </template>
    </b-navbar>
    </div>
</template>
