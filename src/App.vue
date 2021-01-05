<template>
  <layout>
    <add-meal-form />
    <planner />
    <members />
  </layout>
</template>

<script>
import Layout from "./components/Layout.vue";
import AddMealForm from "./components/AddMealForm.vue";
import Members from "./components/Members.vue";
import Planner from "./components/Planner.vue";

export default {
  name: "App",
  components: {
    Layout,
    AddMealForm,
    Planner,
    Members,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin: 0;
  height: 100vh;
  width: 100vw;
}
</style>
