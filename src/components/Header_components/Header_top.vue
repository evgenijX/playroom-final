<template>
  <div class="header_top">
    <Header_language />
    <Header_location />
    <div class="social_icons" style="display: flex;column-gap: 20px">
      <a href="https://www.instagram.com/playroom.kyiv/?utm_medium=copy_link"><img src="../../assets/social-icons/inst.svg" alt=""></a>
      <a href="https://www.facebook.com/playroom.co.ua/"><img src="../../assets/social-icons/fb.svg" alt=""></a>
    </div>
  </div>
</template>

<script>
import Header_language from "@/components/Header_components/Header_language";
import Header_location from "@/components/Header_components/Header_location";
export default {
  name: "Header_top",
  components: {Header_location, Header_language}
}
</script>

<style scoped>
.header_top{
  padding: 10px 10%;
  display: flex;
  justify-content: space-between;
  background-image: url('../../assets/bg/bg_header-top.png');
  background-size: cover;
  background-repeat: no-repeat;
  align-items: center;
}

</style>