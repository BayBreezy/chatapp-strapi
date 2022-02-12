<template>
  <v-menu :close-on-content-click="false" :activator="act" offset-y top>
    <VEmojiPicker @select="$emit('emojiSelected', $event)" />
  </v-menu>
</template>

<script>
import { VEmojiPicker } from "v-emoji-picker";
export default {
  components: {
    VEmojiPicker,
  },
  props: {
    act: String,
  },
};
</script>

<style></style>
