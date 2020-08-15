<template>
  <main class="main">
      <Summoner />
      <Summoner />
      <Summoner />
      <Summoner />
      <Summoner />
  </main>
</template>

<script>
import Summoner from "../components/Summoner";

export default {
  name: "Main",
  components: { Summoner },
};
</script>

<style>
.main {
  grid-area: main;

  display: flex;
  justify-content: space-around;
}
</style>