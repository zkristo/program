<script>
import HomeComponent from './components/HomeComponent.vue';
import Stanice from './components/Stanice.vue';




export default {
  name: 'App',
  components: {
    Stanice,
    HomeComponent
  },
  data() {
    return {
      data: {
        rute: [],
        admins: []
      }
    };
  },
  async created() {
    this.data.rute = await fetch('http://localhost:5000/rute')
      .then(response => response.json())
      .then(data => {
        return data;
      });
    this.data.admins = await fetch('http://localhost:5000/admins')
      .then(response => response.json())
      .then(data => {
        return data;
      });
    localStorage.setItem('currentId', 0)
  }
}
</script>

<template>
  <HomeComponent />
  <Stanice :rute="data.rute" />
</template>

<style scoped></style>
