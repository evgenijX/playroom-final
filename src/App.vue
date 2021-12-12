<template>
  <v-app>
    <Landing />
    <About_us />
    <Timetable />
    <Our_benefits />
    <Why_us />
    <Contact />
  </v-app>
</template>

<script>

import Landing from "@/components/Landing";
import About_us from "@/components/About_us";
import Timetable from "@/components/Timetable";
import Our_benefits from "@/components/Our_benefits";
import Why_us from "@/components/Why_us";
import Contact from "@/components/Contact";

export default {
  name: 'App',

  components: {
    Contact,
    Why_us,
    Our_benefits,
    Timetable,
    About_us,
    Landing,

  },

  data: () => ({
    //
  }),
};
</script>

