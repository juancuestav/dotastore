<template>
  <v-container>
    <v-layout wrap>
      <v-flex v-for="book in books" :key="book.prod_nombre">
        <v-card class="mx-auto" max-width="320" style="margin:10px;">
          <v-img
            height="200"
            src="https://cdn.vuetifyjs.com/images/cards/cooking.png"
          ></v-img>

          <v-card-title>
            <v-row class="mx-5">
              <span class="title blue--text">Producto</span>
              <v-spacer></v-spacer>
              <span class="title"> $ 0.00</span>
            </v-row>
          </v-card-title>

          <v-card-text>
            <div class="mx-5 text-justify">
              Small plates, salads & sandwiches - an intimate setting with 12
              indoor seats plus patio seating.
            </div>
          </v-card-text>

          <v-card-actions class="mx-5">
            <v-btn color="blue-grey accent-3" text> Añadir a carrito </v-btn>
            <v-btn color="blue-grey accent-3" text> Comprar </v-btn>
          </v-card-actions>
        </v-card>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      books: [
        { prod_nombre: "book1", prod_precio: 3, prod_stock: "2016" },
        { prod_nombre: "book2", prod_precio: 3, prod_stock: "2016" },
        { prod_nombre: "book3", prod_precio: 3, prod_stock: "2016" },
        { prod_nombre: "book4", prod_precio: 3, prod_stock: "2016" },
        { prod_nombre: "book5", prod_precio: 3, prod_stock: "2016" },
        { prod_nombre: "book6", prod_precio: 3, prod_stock: "2016" },
      ],
    };
  },
};
</script>
