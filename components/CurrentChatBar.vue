<template>
  <div>
    <v-app-bar elevate-on-scroll app>
      <v-list-item @click="showDialog = true">
        <v-list-item-avatar>
          <v-img src="https://randomuser.me/api/portraits/women/63.jpg"></v-img>
        </v-list-item-avatar>
        <v-list-item-content>
          <v-list-item-title class="text-subtitle-2"
            >Sharon Scott</v-list-item-title
          >
          <v-list-item-subtitle>
            <v-chip dark x-small label color="error">Offline</v-chip>
          </v-list-item-subtitle>
        </v-list-item-content>
      </v-list-item>
      <v-spacer />
      <v-btn icon>
        <v-icon>mdi-dots-vertical</v-icon>
      </v-btn>
    </v-app-bar>
    <ContactDialog :show="showDialog" @CloseContact="showDialog = false" />
  </div>
</template>

<script>
export default {
  data() {
    return {
      showDialog: false,
    };
  },
};
</script>

<style></style>
