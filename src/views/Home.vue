<template>
  <div class="home">
    <Navbar :product="product"/>
    <div class="container">
      <Hero />
      <div class="row mb-4">
        <div
          class="col-md-4 mt-4"
          v-for="product in products"
          :key="product.id"
        >
          <!-- <CardFood :product="product" /> -->
        </div>
      </div>
      </div>
    </div>
</template>

<script>
// @ is an alias to /src
import Navbar from "@/components/Navbar.vue";
import Hero from "@/components/Hero.vue";
import axios from "axios";

export default {
  name: "Home",
  components: {
    Navbar,
    Hero,
  },
  data() {
    return {
      products: [],
    };
  },
  methods: {
    setProducts(data) {
      this.products = data;
    },
  },
  mounted() {
    axios
      .get("http://localhost:3001/api/bestproducts")
      .then((response) => this.setProducts(response.data))
      .catch((error) => console.log(error));
  },
};
</script>
