<template>
  <v-list class="py-1" nav>
    <v-list-item nuxt to="/chat/single/123">
      <v-list-item-avatar>
        <v-img src="https://randomuser.me/api/portraits/women/63.jpg"></v-img>
      </v-list-item-avatar>
      <v-list-item-content>
        <v-list-item-title class="text-subtitle-2"
          >Sharon Scott</v-list-item-title
        >
        <v-list-item-subtitle class="text-caption">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Facilis,
          eligendi error. Nesciunt ipsum asperiores commodi. Cum ea ipsum
          eligendi, amet reiciendis in voluptas esse quod a reprehenderit,
          repudiandae pariatur aut!
        </v-list-item-subtitle>
      </v-list-item-content>
      <v-list-item-action>
        <v-icon size="12" color="green">mdi-circle</v-icon>
      </v-list-item-action>
    </v-list-item>
  </v-list>
</template>

<script>
export default {};
</script>

<style></style>
