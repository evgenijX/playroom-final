<template>
  <v-sheet class="mx-auto slider-component">
    <div class="slider__component-line"></div>
    <v-slide-group v-model="model" show-arrows>
      <v-slide-item v-for="item in items" :key="item.message" style="align-items: center">
        <v-card class="ma-14 slider__card" height="335" width="170" elevation="0">
          <div class="slider__card-img"><img :src="item.img"/></div>
          <div class="slider__card-circle"></div>
          <div class="slider__card-time"
          >
            {{item.time}}
          </div>
          <div class="slider__card-title">{{ item.message }}</div>
        </v-card>
      </v-slide-item>
    </v-slide-group>
  </v-sheet>
</template>

<script>
export default {
  name: "Timetable_young",
  data: () => {
    return ({
      model: null,
      items: [
        { message: "Зустріч дітей, академічна гра ", time: "8:30-9:00", img: require("@/assets/timetable/first.svg")},
        { message: "Сніданок", time: "9:00-9:15" ,img: require("@/assets/timetable/snidanok.svg")},
        { message: "Коло друзів, ранкове вітання", time: "9:15-10:00" ,img: require("@/assets/timetable/circleFriends.svg")},
        { message: "Снєк", time: "10:00-10:10" ,img: require("@/assets/timetable/snek.svg")},
        { message: "English/Гіманстика/French", time: "10:10-10:50" ,img: require("@/assets/timetable/EnglishFrench.svg")},
        { message: "Прогулянка", time: "11:00-11:40" ,img: require("@/assets/timetable/goout.svg")},
        { message: "Розумна дитина/Музика", time: "12:00-12:45" ,img: require("@/assets/timetable/music.svg")},
        { message: "Обід", time: "12:45-12:15" ,img: require("@/assets/timetable/food.svg")},
        { message: "Продовжений день", time: " " },
        { message: "Відпочинок (тиха година)", time: "13:30-15:30" ,img: require("@/assets/timetable/sleep.svg")},
        { message: "Полуденок", time: "15:30-16:00" ,img: require("@/assets/timetable/poludnik.svg")},
        { message: "French/Спорт/Творче зайняття", time: "16:00-16:45" ,img: require("@/assets/timetable/tvorche.png")},
        { message: "Вільна гра", time: "16:50-17:30" ,img: require("@/assets/timetable/freegame.svg")},
        { message: "Вечеря", time: "17:30-18:00" ,img: require("@/assets/timetable/supper.svg")},
        { message: "Вільна гра", time: "18:00-19:00" ,img: require("@/assets/timetable/freegame.svg")}
      ]
    });
  },
}
</script>

<style scoped>
  .slider-component{
    background: none;
    width: 90vw;
  }
  .slider__card{
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    background: none !important;
  }
  .slider__card-time {
    font-weight: 600;
    font-size: 20px;
    text-align: center;
    color: #BEA32E;
    margin-bottom: 10px;
  }
  .slider__card-title{
    width: 166px;
    font-weight: normal;
    font-size: 20px;
    text-align: center;
    color: #000000;
  }
  .slider__card-img{
    width: 115px !important;
    height: 143px !important;
    background: #FFFFFF;
    box-shadow: inset -2px 4px 4px rgba(0, 0, 0, 0.25);
    border-radius: 15px;
    margin: 0 auto;
    display: flex;
    justify-content: center;
    align-content: center;
    align-items: center;
  }
  .slider__component-line{
    content: "";
    max-width: 100%;
    height: 2px;
    background-color: #FFD10B;
    position: relative;
    top: 225px;
    display: flex;
    justify-content: center;
    margin: 0 auto;
  }
  .slider__card-circle {
    width: 18px;
    height: 18px;
    content: "";
    background: #7AD4CB;
    border-radius: 50%;
    margin: 17px auto 8px;
  }
  .v-slide-group__content{
    align-items: flex-start !important;
    display: none;
  }

</style>