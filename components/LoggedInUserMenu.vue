<template>
  <div>
    <v-menu offset-y bottom :activator="activator">
      <v-card>
        <LoggedInUserTile />
        <v-divider />
        <v-list nav>
          <v-list-item nuxt to="/profile">
            <v-list-item-icon>
              <v-icon>mdi-cogs</v-icon>
            </v-list-item-icon>
            <v-list-item-content>
              <v-list-item-title>Settings</v-list-item-title>
            </v-list-item-content>
          </v-list-item>
          <v-list-item nuxt to="/">
            <v-list-item-icon>
              <v-icon color="red">mdi-logout</v-icon>
            </v-list-item-icon>
            <v-list-item-content>
              <v-list-item-title class="red--text">Logout</v-list-item-title>
            </v-list-item-content>
          </v-list-item>
        </v-list>
      </v-card>
    </v-menu>
  </div>
</template>

<script>
export default {
  props: {
    activator: String,
  },
};
</script>

<style></style>
