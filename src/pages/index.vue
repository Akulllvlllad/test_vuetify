<template>
  <div class="wrapper">

    <v-carousel class="UCarousel" cycle hide-delimiter-background show-arrows="hover">
      <v-carousel-item
      class="UCarousel__item"
        src="https://cdn.vuetifyjs.com/images/cards/docks.jpg"
        cover
      ></v-carousel-item>

      <v-carousel-item
        src="https://cdn.vuetifyjs.com/images/cards/hotel.jpg"
        cover
      ></v-carousel-item>

      <v-carousel-item
        src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
        cover
      ></v-carousel-item>
    </v-carousel>





    <section class="USection section">
      <div class="container grid">
        <v-hover v-slot="{ isHovering, props }" v-for="i of 10" :key="i">
          <v-card
            class="mx-auto"
            color="grey-lighten-4"
            max-width="600"
            v-bind="props"
          >
            <v-img
              :aspect-ratio="16/9"
              cover
              src="https://cdn.vuetifyjs.com/images/cards/kitchen.png"
            >
              <v-expand-transition>
                <div
                  v-if="isHovering"
                  class="d-flex transition-fast-in-fast-out bg-orange-darken-2 v-card--reveal text-h2"
                  style="height: 100%;"
                >
                  400₽
                </div>
              </v-expand-transition>
            </v-img>

            <v-card-text class="pt-6">
              <div class="font-weight-light text-grey text-h6 mb-2">
                For the perfect meal
              </div>

              <h3 class="text-h4 font-weight-light text-orange mb-2">
                QW cooking utensils
              </h3>

              <div class="font-weight-light text-h6 mb-2">
                Our Vintage kitchen utensils delight any chef.<br>
                Made of bamboo by hand
              </div>
            </v-card-text>
          </v-card>
        </v-hover>
      </div>
    </section>













    <div class="container section">
      <v-expansion-panels>
        <v-expansion-panel
          title="Title"
          text="Lorem ipsum dolor sit amet consectetur adipisicing elit. Commodi, ratione debitis quis est labore voluptatibus! Eaque cupiditate minima"
        >
        </v-expansion-panel>
        <v-expansion-panel
          title="Title"
          text="Lorem ipsum dolor sit amet consectetur adipisicing elit. Commodi, ratione debitis quis est labore voluptatibus! Eaque cupiditate minima"
        >
        </v-expansion-panel>
        <v-expansion-panel
          title="Title"
          text="Lorem ipsum dolor sit amet consectetur adipisicing elit. Commodi, ratione debitis quis est labore voluptatibus! Eaque cupiditate minima"
        >
        </v-expansion-panel>
        <v-expansion-panel
          title="Title"
          text="Lorem ipsum dolor sit amet consectetur adipisicing elit. Commodi, ratione debitis quis est labore voluptatibus! Eaque cupiditate minima"
        >
        </v-expansion-panel>
      </v-expansion-panels>
    </div>


    
  </div>
</template>

<script setup lang="ts">
 
</script>

<style scoped>
.container{
  max-width: 1200px;
  margin: 0 auto;
}

.grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(260px, 1fr));
  gap: 30px 10px; /* Расстояние между элементами (по желанию) */
}

.item {
  /* Стили для элементов внутри грида */
  border: 1px solid #ccc;
  padding: 10px;
  text-align: center;
}

.USection{
  
}
.section{
  padding: 60px 0px;
}

.UCarousel{
  height: 70vh !important;
  
}
.UCarousel__item{
    
  }
</style>


