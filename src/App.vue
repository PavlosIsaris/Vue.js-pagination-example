<template>
  <div id="app">
    <pagination-component></pagination-component>
  </div>
</template>

<script>
import PaginationComponent from './components/PaginationComponent.vue'
import 'bootstrap';

export default {
  name: 'app',
  components: {
    PaginationComponent
  }
}
</script>

<style>
  @import "~bootstrap/dist/css/bootstrap.min.css";
</style>
