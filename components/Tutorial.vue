<!-- Please remove this file from your project -->
<template>
  <!-- <v-row justify="center">
      <v-card class="mx-auto" width="256" tile>
        <v-navigation-drawer permanent>
          <v-system-bar></v-system-bar>
          <v-list>
            <v-list-item>
              <v-list-item-avatar>
                <v-img src="https://cdn.vuetifyjs.com/images/john.png"></v-img>
              </v-list-item-avatar>
            </v-list-item>

            <v-list-item link>
              <v-list-item-content>
                <v-list-item-title class="text-h6">
                  JHONATAN STIWAR GAITAN PABON
                </v-list-item-title>
                <v-list-item-subtitle
                  >gaitan2266@hotmail.com</v-list-item-subtitle
                >
              </v-list-item-content>

              <v-list-item-action>
                <v-icon>mdi-menu-down</v-icon>
              </v-list-item-action>
            </v-list-item>
          </v-list>
          <v-divider></v-divider>
          <v-list nav dense>
            <v-list-item-group v-model="selectedItem" color="primary">
              <v-list-item v-for="(item, i) in items" :key="i">
                <v-list-item-icon>
                  <v-icon v-text="item.icon"></v-icon>
                </v-list-item-icon>

                <v-list-item-content>
                  <v-list-item-title v-text="item.text"></v-list-item-title>
                </v-list-item-content>
              </v-list-item>
            </v-list-item-group>
          </v-list>
        </v-navigation-drawer>
      </v-card>
    </v-row> -->

  <v-carousel>
    <v-carousel-item
      v-for="(item, i) in items"
      :key="i"
      :src="item.src"
      reverse-transition="fade-transition"
      transition="fade-transition"
    ></v-carousel-item>
  </v-carousel>
</template>


<script>
export default {
  data: () => ({
    selectedItem: 0,
    /* items: [
      { text: "Mis Archivos", icon: "mdi-folder" },
      { text: "Compartidos conmigo", icon: "mdi-account-multiple" },
      { text: "Favoritos", icon: "mdi-star" },
      { text: "Recientes", icon: "mdi-history" },
      { text: "Sin internet", icon: "mdi-check-circle" },
      { text: "Subidas", icon: "mdi-upload" },
      { text: "Guardar en la nube", icon: "mdi-cloud-upload" },
    ], */

    items: [
      {
        src: "https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg",
      },
      {
        src: "https://cdn.vuetifyjs.com/images/carousel/sky.jpg",
      },
      {
        src: "https://cdn.vuetifyjs.com/images/carousel/bird.jpg",
      },
      {
        src: "https://cdn.vuetifyjs.com/images/carousel/planet.jpg",
      },
    ],
  }),
};
</script>