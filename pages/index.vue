<template>
  <v-container class="fill-height">
    <v-row align="center" justify="center">
      <v-col cols="12" md="4">
        <v-card class="pa-5 el" rounded="lg">
          <h1 class="text-center">Login</h1>
          <br /><br /><br />
          <v-row no-gutters>
            <v-col cols="12">
              <v-text-field outlined type="email" label="Email"></v-text-field>
            </v-col>
            <v-col cols="12">
              <v-text-field
                outlined
                type="password"
                label="Password"
              ></v-text-field>
            </v-col>
            <v-col cols="12">
              <v-btn block color="primary" min-height="50">Login</v-btn>
            </v-col>
            <v-col cols="12">
              <br />
              <div class="d-flex">
                <p class="text-caption primary--text pointer">
                  Forgot password?
                </p>
                <v-spacer />
                <p
                  @click="$router.push('/register')"
                  class="text-caption primary--text pointer"
                >
                  Register
                </p>
              </div>
            </v-col>
          </v-row>
        </v-card>
      </v-col>
      <v-spacer />
      <v-col md="7">
        <v-img src="/icon.png"></v-img>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {};
</script>

<style></style>
