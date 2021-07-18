<template>
    <div class="app-top-bar">
        <v-app-bar app
      color="dark darken-4" dark>
      <v-app-bar-nav-icon @click="drawer = true"></v-app-bar-nav-icon>

      <v-toolbar-title>Kit Quebrada</v-toolbar-title>

    </v-app-bar>

    <v-navigation-drawer
      v-model="drawer"
      absolute
      temporary
    >
      <v-list
        nav
        dense
      >
        <v-list-item-group
          v-model="group"
          active-class="brown darken-4"
        >
          <v-list-item>
            <v-list-item-icon>
              <v-icon>mdi-basket-fill</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Solicitar Cesta</v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-icon>
              <v-icon>mdi-basket-unfill</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Doar Cesta</v-list-item-title>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>
    </div>
    
</template>

<script>
export default {
    name: "AppTopBar",
    data: () => ({
        drawer: false,
        group: null,
    })
}
</script>