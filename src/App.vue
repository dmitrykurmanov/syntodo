<template>
    <div>
        <header>
            <nav>
                <router-link to="/" exact>go to main!</router-link>
                <router-link to="/home">Home</router-link>
                <router-link to="/todos">Todos</router-link>
                <router-link to="/calendar">Calendar</router-link>
                <router-link to="/chat">Chat</router-link>
            </nav>
        </header>
        <transition name="fade" mode="out-in">
            <router-view></router-view>
        </transition>
    </div>
</template>

<script>
    import Vue from 'vue'
    import {Component} from 'vue-property-decorator'

    @Component
    export default class App extends Vue {}
</script>


