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
  <!-- <div>
    <pre>{{ JSON.stringify(formData, null, 2) }}</pre>
  </div>
  <form @submit="submit">
    <div><label for="name">Name</label> <br /><input type="text" id="name" v-model="formData.name" class="border-3"></div>
    <div><label for="email">Email</label><br /><input type="email" id="email" v-model="formData.email" class="border-3">
    </div>
    single select dropdown
    <div><label for="country">country</label> <select id="country" v-model="formData.country">
        <option value="">Select country</option>
        <option value="Sudan">sudan</option>
        <option value="USA">USA</option>
        <option value="KSA">KSA</option>
      </select></div>
    multiple select dropdown
    <div><label for="country">jobLocation</label> <select id="jobLocation" multiple v-model="formData.jobLocation">
        <option value="Sudan">sudan</option>
        <option value="USA">USA</option>
        <option value="KSA">KSA</option>
      </select></div>
    single checkbox
    <div> <input type="checkbox" id="checkbox" v-model="formData.checkbox"> <label for="checkbox">single checkbox</label>
    </div>
    multi checkbox
    <div> <input type="checkbox" id="html" value="html" v-model="formData.skils"> <label for="html">html</label>
      <input type="checkbox" id="css" value="css" v-model="formData.skils"> <label for="css">css</label>
      <input type="checkbox" id="js" value="js" v-model="formData.skils"> <label for="js">js</label>
      <input type="checkbox" id="flutter" value="flutter" v-model="formData.skils"> <label for="flutter">flutter</label>
    </div>
    radio
    <div><label for="0-2">0-2</label> <input type="radio" value="0-2" id="0-2" v-model="formData.yearofexp"><label
        for="3-6">3-6</label> <input type="radio" value="3-6" id="3-6" v-model="formData.yearofexp"></div>
    <div><button>submit</button></div>
  </form> -->
  <!-- Component
  <Hello name="fadwa" :lastName="lastName" age=24 uniName="uofk" /> -->
  <!-- Slot -->
  <!-- <Card content="content 1" />
  <Card content="content 2" /> -->
  <!-- <Card>Hi slot</Card> -->
  <!-- <Layout>
    <template v-slot:header>
      <h1>Header</h1>
    </template>
    <template v-slot:content>
      <h1>content</h1>
    </template>
    <template v-slot:footer>
      <h1>footer</h1>
    </template>
  </Layout> -->
  <div class="align-middle text-center"> Dynamic component

    <button @click="activeComponent = 'TabA'">TabA</button>
    <button @click="activeComponent = 'TabB'">TabB</button>
    <button @click="activeComponent = 'TabC'">TabC</button>
    <component :is="activeComponent" />
    <!-- <TabA />
    <TabB />
    <TabC /> -->
  </div>
</template>


<script >
import Hello from "./components/Hello.vue"
import Card from "./components/Card.vue"
import Layout from "./components/Layout.vue"
import TabA from "./components/TabA.vue"
import TabB from "./components/TabB.vue"
import TabC from "./components/TabC.vue"
export default {
  components: { Hello, Card, Layout, TabA, TabB, TabC },
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
      // formData: {
      //   name: "",
      //   email: "",
      //   country: "",
      //   jobLocation: [],
      //   checkbox: false,
      //   skils: [],
      //   yearofexp: "",
      // }
      // lastName: 'Ali'
      activeComponent: 'TabA'
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
    // submit(event) {
    //   event.preventDefault()
    //   console.log('form values', this.formData)

    // }
  }
}
</script>