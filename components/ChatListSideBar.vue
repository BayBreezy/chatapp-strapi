<template>
  <div>
    <v-navigation-drawer width="300" app permanent>
      <LoggedInUserTile id="usertile" />
      <v-text-field
        outlined
        dense
        class="ma-3 text-body-2"
        hide-details="auto"
        placeholder="Search"
      ></v-text-field>
      <SingleChatTile />
      <GroupChatTile />
      <SingleChatTile />
      <GroupChatTile />
      <SingleChatTile />
      <GroupChatTile />
      <SingleChatTile />
      <GroupChatTile />
      <SingleChatTile />
      <GroupChatTile />
      <SingleChatTile />
      <GroupChatTile />
      <SingleChatTile />
      <GroupChatTile />
    </v-navigation-drawer>
    <LoggedInUserMenu activator="#usertile" />
  </div>
</template>

<script>
export default {};
</script>

<style></style>
