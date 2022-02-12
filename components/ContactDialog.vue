<template>
  <div>
    <v-dialog width="400" v-model="dialog">
      <v-card rounded="lg" class="pa-5 text-center">
        <v-btn @click="dialog = false" absolute top right icon small>
          <v-icon small>mdi-close</v-icon>
        </v-btn>
        <v-avatar size="130">
          <v-img src="https://randomuser.me/api/portraits/women/63.jpg"></v-img>
        </v-avatar>
        <p class="mt-7">Sarah Scott</p>
        <a class="text-body-2" href="mailto:sarahscott@test.com"
          >sarahscott@test.com</a
        >
      </v-card>
    </v-dialog>
  </div>
</template>

<script>
export default {
  props: {
    user: Object,
    show: Boolean,
  },
  computed: {
    dialog: {
      get() {
        return this.show;
      },
      set(v) {
        this.$emit("CloseContact");
      },
    },
  },
};
</script>

<style></style>
