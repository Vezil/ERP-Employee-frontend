<template>
    <v-app class="grey">
        <Navbar />
        <v-main>
            <transition name="router-anim" enter-active-class="animated pulse">
                <router-view />
            </transition>
        </v-main>
    </v-app>
</template>

<script>
import Navbar from './components/Navbar';

export default {
    name: 'App',

    components: {
        Navbar
    },

    data: () => ({
        //
    })
};
</script>
<style>
@import 'https://cdn.jsdelivr.net/npm/animate.css@3.5.1';

.page {
    width: inherit;
    background-image: url('img/background.jpg') !important;
}
</style>
