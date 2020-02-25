<template>
  <Layout>
      <v-container
        class="fill-height"
        fluid
      >
        <v-row
          align="center"
          justify="center"
        >
          <v-col class="text-center">
            <g-image alt="gridsome logo" src="~/favicon.png" width="135" />
            <g-image alt="vuetify logo" src="~/vuetify-logo-dark.webp" width="135" />
          </v-col>
        </v-row>
      </v-container>
  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: 'Hello, world!'
  }
}
</script>

<style>
.home-links a {
  margin-right: 1rem;
}
</style>
