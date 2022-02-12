<template>
  <v-container ref="msg" class="">
    <ChatListSideBar />
    <CurrentChatBar />
    <div v-for="n in 30" :key="`msg${n}`">
      <SenderChatBubble v-if="n % 2 == 0" />
      <SenderChatBubbleImage v-if="n == 29" />
      <MyChatBubbleImage v-if="n == 27" />
      <MyChatBubbleFile v-if="n == 28" />
      <MyChatBubble v-else />
    </div>
    <div id="end"></div>
    <ChatInput />
  </v-container>
</template>

<script>
export default {
  mounted() {
    this.ScrollEnd();
  },
  methods: {
    ScrollEnd() {
      // this.$refs.msg?.scrollIntoView({ behavior: "smooth", block: "end" });

      this.$vuetify.goTo("#end", { duration: 100 });
    },
  },
};
</script>

<style></style>
