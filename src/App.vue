<template>
  <Navbar/>
  <Donnee/>
  <Modal/>
</template>

<script>
import Donnee from './components/Donnee.vue'
import Modal from './components/Modal.vue'
import Navbar from './components/Navbar.vue';


export default {
  name: 'App',
  components: {
    Donnee,
    Modal,
    Navbar
}
}
</script>

<style>
   @import '../style.css';
</style>
