<template lang="">
    <div>
        <div class="mt-8">
            <NavList :header_navbar=true :page_selection="page_selection" :nav_inline=false :items="nav_menu" />
        </div>
    </div>
</template>
<script>
import NavList from './NavList.vue';

export default {
    components: {    
        NavList,
    },
    props:{
        page_selection: String,
    },
    data() {
        return {
            nav_menu: [
                {
                    title:'Dashboard',
                    id:'admin/dashboard'
                },
                {
                    title:'Pessoas',
                    id:'admin/people'
                },
                {
                    title:'Meus Eventos',
                    id:'admin/my-events'
                },
                {
                    title:'Vendas',
                    id:'admin/sales'
                },
                {
                    title:'Configurações',
                    id:'admin/settings'
                }
            ]
        }
    },
}
</script>
<style lang="">
    
</style>