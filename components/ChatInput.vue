<template>
  <v-footer app inset>
    <v-btn @click="$refs.hiddenInput.click()" icon>
      <v-icon size="18">mdi-paperclip</v-icon>
    </v-btn>
    <v-btn id="ebtn" icon>
      <v-icon size="18">mdi-emoticon</v-icon>
    </v-btn>
    <v-text-field
      clearable
      @click:clear="file = null"
      prepend-inner-icon="mdi-file"
      :value="file.name"
      hide-details="auto"
      readonly
      filled
      v-if="file"
    >
    </v-text-field>
    <v-textarea
      full-width
      v-else
      hide-details="auto"
      filled
      rows="1"
      v-model="message"
      class="mx-3"
      placeholder="type here"
    ></v-textarea>

    <v-btn icon>
      <v-icon size="18">mdi-send</v-icon>
    </v-btn>
    <EmojiPicker act="#ebtn" @emojiSelected="emojiSelected" />
    <input
      type="file"
      hidden
      ref="hiddenInput"
      @change="loadFile"
      @click="$event.target.value = ''"
    />
  </v-footer>
</template>

<script>
export default {
  data() {
    return {
      message: "",
      file: null,
    };
  },
  methods: {
    emojiSelected(emoji) {
      this.message += emoji.data;
    },
    loadFile(e) {
      const file = e.target.files[0];
      if (!file) return;
      this.file = file;
    },
  },
};
</script>

<style></style>
