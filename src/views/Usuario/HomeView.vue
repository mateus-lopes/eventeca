<template>
  <div>
    <header>
      <NavbarComp page_selection="/" />
      <section class="container max-w-7xl mx-auto pt-3">
        <InfoAlert
          text="Desing Interativo, arraste para o lado com o mouse ou touch para navegar"
          type="info"
        />
      </section>
    </header>
    <main class="container max-w-7xl mx-auto mb-20">
      <section class="mt-4">
        <CategoriesList></CategoriesList>
      </section>
      <section class="mt-6">
        <TitleList>Eventos em Destaque</TitleList>
        <EventsSpecial></EventsSpecial>
      </section>
      <section class="my-8">
        <TitleList>
          <router-link to="/teste"> Categoria 1 </router-link>
        </TitleList>
        <EventsList></EventsList>
      </section>
      <section>
        <TitleList>Categoria 2</TitleList>
        <EventsList></EventsList>
      </section>
      <section class="mb-16 mt-8">
        <TitleList>Categoria 3</TitleList>
        <EventsList></EventsList>
      </section>
      <AdvantagesSection></AdvantagesSection>
      <section class="mt-16">
        <FriendsSection></FriendsSection>
      </section>
    </main>
    <footer>
      <Footer page_selection="/"></Footer>
    </footer>
  </div>
</template>

<script>
import CategoriesList from "../../components/Event/CategoriesList.vue";
import EventsList from "../../components/Event/EventsList.vue";
import EventsSpecial from "../../components/Event/EventsSpecial.vue";
import Footer from "../../components/Footer/FooterComp.vue";
import NavbarComp from "../../components/Navbar/NavComp.vue";
import TitleList from "../../components/Commun/TitleList.vue";
import AdvantagesSection from "../../components/Commun/AdvantagesSection.vue";
import FriendsSection from "../../components/Commun/FriendsSection.vue";
import InfoAlert from "../../components/Commun/InfoAlert.vue";

export default {
  data() {
    return {};
  },
  components: {
    NavbarComp,
    TitleList,
    Footer,
    CategoriesList,
    EventsSpecial,
    EventsList,
    AdvantagesSection,
    FriendsSection,
    InfoAlert,
  },
};
</script>

<style scoped></style>
