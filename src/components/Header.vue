<template>
  <div class="header">
    <Header_top />
    <Header_bottom />
  </div>
</template>

<script>
import Header_top from "@/components/Header_components/Header_top";
import Header_bottom from "@/components/Header_components/Header_bottom";
export default {
  name: "Header",
  components: {Header_bottom, Header_top}
}
</script>

<style scoped>

</style>