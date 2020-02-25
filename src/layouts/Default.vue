<template>
  <v-app>
    <v-navigation-drawer
      v-model="drawer"
      app
    >
      <v-list>
        <v-list-item link to="/">
          <v-list-item-content>
            Home
          </v-list-item-content>
        </v-list-item>
        <v-list-item link to="/about">
          <v-list-item-content>
            About
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>

    <v-app-bar app>
      <v-app-bar-nav-icon @click.stop="drawer = !drawer" />
      <v-toolbar-title>{{ $static.metadata.siteName }}</v-toolbar-title>
    </v-app-bar>

    <v-content>
        <slot/>
    </v-content>

    <v-footer app>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data: () => ({
    drawer: null,
  })
}
</script>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

