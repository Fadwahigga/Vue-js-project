<template>
  <!-- <div class=" justify-center border p-60">  -->
  <!-- <div class="text-3xl font-bold underline bg-red-600">Hello {{ name }}</div>
  <div class="text-3xl font-bold underline bg-blue-500" v-text="name"></div> -->
  <!-- <h1 v-if="num == 0">The Number is zero</h1>
  <h1 v-else-if="num > 0">The Number is positive</h1>
  <h1 v-else-if="num < 0">The Number is nagative</h1>
  <h1 v-else>The Number is not zero</h1>
  <h1 v-show="show">Show element</h1>
  <h1 v-for="name in names" :key="name">{{ name }}</h1> -->
  <!-- <h1 v-for="name in fullNames" :key="name.frst">{{ name.frst }} {{ name.last }}</h1> -->
  <!-- <div v-for="actor in actors" :key="actor.name">
    <h1>{{ actor.name }}</h1>
    <h1 v-for="movie in actor.movies" :key="movie">{{ movie }}</h1>
  </div> -->
  <!-- <h1 v-for="(value , key ,index) in infVal" :key="value"> {{ index }} {{ key }}{{ value }}</h1> -->
  <!-- <h1>{{ add ()}}</h1>
  <h1>{{ multi() }}</h1>
  <h1>{{ passdata(multvar) }}</h1> -->
  <!-- <h1>{{ name }}</h1>
    <button v-on:click="name = 'Ali'">Change name</button>
    <h1>{{ num }}</h1>
    <button @click="num = num + 1">Increes</button>
    <br/>
    <button v-on:click="decrement" class="bg-red-600">decreement</button>
    <br/>
    <button v-on:click="increement(3)" class="bg-red-600">increement by method</button> -->
  <!-- </div> -->
  <form>
    <div><label for="name">Name</label> <br/><input type="text" id="name" v-model="formData.name" class="border-3"></div>
    <div><label for="email">Email</label><br/><input type="email" id="email" v-model="formData.email" class="border-3"></div>
  </form>
</template>


<script >
export default {
  data() {
    return {
      // name: "fadwa",
      // num: -7,
      // show:false,
      // names:["fadwa","ali","foff"],
      // fullNames: [{ frst: "fadwa", last: "ali" }, { frst: "ali", last: "fadl" }, { frst: "fadl", last: "higga" }],
      // actors: [{ name: "fadwa", movies: ["first", "secend"] }, { name: "Ali", movies: ["ali first", "ali secend"] }]
      // infVal: { name: "fadwa", chanel: "fadwaaa", course: "vuejs" }
      // multvar: 3
      formData: {
        name: "",
        email: ""
      }
    }
  },
  methods: {
    // add() {
    //   return 5 + 5
    // },
    // multi() {
    //   return this.multvar * 2
    // }
    // , passdata(a) {
    //   return a;
    // }
    // decrement() {
    //   this.num = this.num - 1
    // },
    // increement(x){
    //   this.num += x
    // }
  }
}
</script>