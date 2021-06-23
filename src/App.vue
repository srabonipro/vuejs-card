<template>
<div>
  
  <h1 class="text-danger">Learning About Slots</h1>
  <!-- card 1 -->
  <Card />

  <!-- card 2 -->
  <Card>
     <template #footer>
      <p><a href="#">card footer</a></p>
    </template>
  </Card>

  <!-- card 3 -->
  <Card>
    <template #header>
      <h1>Product Title</h1>
    </template>
    <template #body>
      <img src="https://randomuser.me/api/portraits/men/79.jpg" alt="">
      <p>
        <ul>
          <li>Lorem ipsum dolor sit amet.</li>
          <li>Lorem ipsum dolor sit amet.</li>
          <li>Lorem ipsum dolor sit amet.</li>
        </ul>
      </p>
    </template>
    <template #footer>
      <div class="d-flex gap-2 justify-content-center">
        <button class="btn btn-sm btn-info">Buy</button>
        <button class="btn btn-sm btn-success">Cart</button>
      </div>
    </template>
  </Card>

</div>
</template>

<script>
import Card from './components/Card.vue'

export default {
  name: 'App',
  components: {
    Card,
  },
  data() {
    return {
    }
  },

}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
