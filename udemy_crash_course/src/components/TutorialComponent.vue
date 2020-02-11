<template>
  <div id="my-app">
    <h1>
      Hey There
      {{
        name
          .split("")
          .reverse()
          .join("")
      }}! How's it like in New York City!?
    </h1>

    <h1>Counter Example</h1>
    <h2>Counter: {{ counter }}</h2>

    <button @click="increase">Increase</button>
    <br />

    <img :src="imgSrc" />
    <hr />
  </div>
</template>

<script>
export default {
  name: "TutorialComponent",
  props: ["name", "imgSrc"],
  data: function() {
    return {
      counter: 0
    };
  },
  methods: {
    increase: function() {
      this.counter += 1;
    }
  }
};
</script>

<style scoped></style>
