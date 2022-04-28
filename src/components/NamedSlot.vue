<template>
  <div>
    <header><slot name="header" msg="from header"></slot></header>
    <footer><slot name="footer"></slot></footer>
  </div>
</template>

<script>
export default {
  name: "namedslot",
};
</script>