<template lang="">
    <div class="bg-gray-100 min-h-screen flex gap-16">
        <header class="hidden w-full lg:w-3/12 bg-primary relative lg:bg-white lg:shadow-lg h-screen lg:flex flex-col justify-center lg:justify-start items-center pt-16">
            <nav class="p-12 border-b">
                <img src="../../assets/img/logo.png" class="h-14" alt="">
            </nav>
            <NavCompAdmin page_selection="admin/events/settings" />
            <!-- rodape -->
            <BtnFooterAdmin link="/admin/dashboard">
                Voltar ao Dashboard 
            </BtnFooterAdmin>
        </header>
        <div class="w-full lg:w-9/12 pt-16">
            <main>
                <Paginator text1="Evento" text="Configurações" />
                <!-- conteudo -->
               
            </main>
        </div>
    </div>
</template>
<script>
import NavCompAdmin from "../../components/Navbar/NavDashEvent.vue";
import BtnUserAdmin from "../../components/Navbar/BtnUserAdmin.vue";
import BtnFooterAdmin from "../../components/Footer/BtnFooterAdmin.vue";
import Paginator from "../../components/Commun/Paginator.vue";
import CardDash from "../../components/Commun/CardDash.vue";
import BigCardDash from "../../components/Commun/BigCardDash.vue";
import BigBigCardDash from "../../components/Commun/BigBigCardDash.vue";

export default {
    components: {
        NavCompAdmin,
        BtnFooterAdmin,
        BtnUserAdmin,
        Paginator,
        CardDash,
        BigCardDash,
        BigBigCardDash
    }
}
</script>