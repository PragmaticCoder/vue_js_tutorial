<template>
  <div id="my-app">
    <h1>Hey There {{ name.split('').reverse().join('')}}! How's it like in New York City!?</h1>
  </div>
</template>

<script>
export default {
  name: "TutorialComponent",
  props: ["name"]
};
</script>

<style scoped></style>
