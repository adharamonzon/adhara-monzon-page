<template>
  <HeaderComponent/>
  <AboutMeComponent />
  <ProjectsMenu />
  <SocialMedia />
  <ContactComponent />
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import HeaderComponent from '../components/HeaderComponent.vue';
import AboutMeComponent from '../views/AboutMeComponent.vue';
import ProjectsMenu from './ProjectsMenu.vue';
import SocialMedia from './SocialMedia.vue';
import ContactComponent from './ContactComponent.vue';

export default defineComponent({
  name: 'Landing',
  components: {
    HeaderComponent,
    AboutMeComponent,
    ProjectsMenu,
    SocialMedia,
    ContactComponent
  }
})
</script>

<style lang="css">
.header {
  height: 100vh;
  background-image: url('../assets/images/header.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-around;
}
.header-titleContainer {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: 8.12rem;
}
.header-logo {
  width: 18.87rem;
  height: 9.37rem;
}
.header-title {
  font-size: 5rem;
  font-weight: normal;
  color: white;
  margin-top: 1.75rem;
  letter-spacing: 0.56rem;
}
.header-subtitle {
  font-size: 1.87rem;
  font-weight: normal;
  color: white;
  margin-top: 1.75rem;
  line-height: 1.07;
  letter-spacing: 1.125rem;
}
.nav {
  width: 70%;
  justify-content: center;
}
.nav-list {
  list-style: none;
  display: flex;
  justify-content: space-evenly;
  font-size: 1.25rem;
  padding: 0.31rem;
  cursor: pointer;
  width: 55%;
}
.nav-item-item-link {
  text-decoration-line: none;
  color: white;
  border: 0.18rem solid transparent;
}
.nav-item-item-link:hover {
  border-bottom: 0.18rem solid #9bd189;
  color: white;
}
</style>