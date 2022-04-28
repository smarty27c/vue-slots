<template>
  <div id="app">
    <HelloWorld v-slot="slotProps" nm="fff">
      my name is suraj {{ slotProps.msgs }}</HelloWorld
    >
    <NamedSlot>
      <template #header="headerProps">
        I am in header {{ headerProps.msg }}</template
      >
      <template slot="footer"> I am in footer</template>
    </NamedSlot>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld";
import NamedSlot from "./components/NamedSlot";

export default {
  name: "App",
  components: {
    HelloWorld,
    NamedSlot,
  },
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
