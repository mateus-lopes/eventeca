<template lang="">
    <div @click="goEvent" class="bg-white cursor-pointer p-2">
        <div>
            <a href="#">
                <img class="rounded-2xl w-full" src="../../assets/img/example.jpg" alt="">
            </a>
        </div>
        <div class="">
            <router-link to="/">
                <TitleH1 size="xl" title="Titulo do Evento" />
            </router-link>
            <p class="font-light text-sm">
                Segunda Feira, 9 de julho de 2022
            </p>
        </div>
    </div>
    <!-- <img :src="returnImg()" class="cursor-pointer md:hidden w-full" alt=""> -->
</template>

<script>
import TitleH1 from '../Commun/TitleH1.vue';

export default {
    props: {
        event: Object,
    },
    methods: {
        goEvent() {
            this.$router.push(`/event/`)
        },    
            // returnImg(){
            //     return `https://image.tmdb.org/t/p/w500/${this.movie.poster_path}`
            // }
    },
    components: {
        TitleH1,
    }
    }
</script>