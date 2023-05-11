

<template>
  <!-- <div class="text-3xl font-bold underline bg-red-600">Hello {{ name }}</div>
  <div class="text-3xl font-bold underline bg-blue-500" v-text="name"></div> -->
  <!-- <h1 v-if="num == 0">The Number is zero</h1>
  <h1 v-else-if="num > 0">The Number is positive</h1>
  <h1 v-else-if="num < 0">The Number is nagative</h1>
  <h1 v-else>The Number is not zero</h1>
  <h1 v-show="show">Show element</h1>
  <h1 v-for="name in names" :key="name">{{ name }}</h1> -->
  <!-- <h1 v-for="name in fullNames" :key="name.frst">{{ name.frst }} {{ name.last }}</h1> -->
  <div v-for="actor in actors" :key="actor.name">
    <h1>{{ actor.name }}</h1>
    <h1 v-for="movie in actor.movies" :key="movie">{{ movie }}</h1>
  </div>
</template>


<script >
export default {
  data() {
    return {
      // name: "fadwa" ,
      // num :-7,
      // show:false,
      // names:["fadwa","ali","foff"],
      // fullNames: [{ frst: "fadwa", last: "ali" }, { frst: "ali", last: "fadl" }, { frst: "fadl", last: "higga" }],
      actors: [{ name: "fadwa", movies: ["first", "secend"] }, { name: "Ali", movies: ["ali first", "ali secend"] }]
    }
  }
}
</script>