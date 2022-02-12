<template>
  <v-container>
    <ChatListSideBar />
    <br /><br />
    <v-avatar class="mx-auto d-block" size="200">
      <v-img src="https://behonbaker.com/behonbaker.png">
        <v-row class="fill-height" align="end" justify="center">
          <v-btn fab small depressed color="primary">
            <v-icon small>mdi-camera</v-icon>
          </v-btn>
        </v-row>
      </v-img>
    </v-avatar>
    <br /><br />
    <v-row align="center" justify="center">
      <v-col cols="12" md="4">
        <v-row no-gutters>
          <v-col cols="12">
            <v-text-field outlined type="text" label="Name"></v-text-field>
          </v-col>
          <v-col cols="12">
            <v-text-field outlined type="email" label="Email"></v-text-field>
          </v-col>
          <v-col cols="12">
            <v-text-field
              outlined
              type="password"
              label="New Password"
            ></v-text-field>
          </v-col>
          <v-col cols="12">
            <v-btn min-width="120" color="primary" min-height="45"
              >Update</v-btn
            >
          </v-col>
        </v-row>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {};
</script>

<style></style>
