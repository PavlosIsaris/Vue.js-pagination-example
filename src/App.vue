<template>
  <div id="app">
    <div class="mt-5">
      <pagination-component v-bind:steps="steps">
        <template v-slot:content_0>
          <h2>This is our first step!</h2>
          <img src="../public/img/1.gif">
        </template>
        <template v-slot:content_1>
          <h2>Second step here!</h2>
          <img src="../public/img/2.gif">
        </template>
        <template v-slot:content_2>
          <h2>Another cool step</h2>
          <img src="../public/img/3.gif">
        </template>
        <template v-slot:content_3>
          <h2>Final and best step...</h2>
          <img src="../public/img/4.gif">
        </template>
      </pagination-component>
    </div>
  </div>
</template>

<script>
import PaginationComponent from './components/PaginationComponent.vue'
import 'bootstrap';

export default {
  name: 'app',
  components: {
    PaginationComponent
  },
  data() {
    return {
      steps: [
        {
          title: 'Introduction',
          allowNext: false
        }, {
          title: 'Second',
          allowNext: false
        }, {
          title: 'Third',
          allowNext: false
        }, {
          title: 'Final',
          allowNext: false
        }
      ]
    }
  }
}
</script>

<style lang="scss">
  @import "~bootstrap/dist/css/bootstrap.min.css";

  h2{
    margin-bottom: 2rem;
  }

  img {
    height: 250px;
  }

</style>
