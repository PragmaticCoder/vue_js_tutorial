<template>
  <div id="my-app">
    <h1 v-text="message"></h1>
  </div>
</template>

<script>
export default {
  name: "TutorialComponent",
  data: function() {
    return {
      message: "Hello Vue"
    };
  }
};
</script>

<style scoped></style>
