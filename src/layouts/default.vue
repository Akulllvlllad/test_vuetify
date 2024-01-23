<template>
  <v-app>
    
    <DefaultBar />

    <DefaultView />

    <v-footer class="footer d-flex flex-column">
      <div class="bg-teal d-flex w-100 align-center px-4">
        <strong>Get connected with us on social networks!</strong>

        <v-spacer></v-spacer>

        <v-btn
          v-for="icon in icons"
          :key="icon"
          class="mx-4"
          :icon="icon"
          variant="plain"
          size="small"
        ></v-btn>
      </div>

      <div class="px-4 py-2 bg-black text-center w-100">
        {{ new Date().getFullYear() }} — <strong>Кристина</strong>
      </div>
    </v-footer>
  </v-app>
</template>

<script lang="ts" setup>
  import DefaultBar from './default/AppBar.vue'
  import DefaultView from './default/View.vue'
</script>

<style scoped>
.footer{
  padding: 0px !important;
}


</style>