<template>
  <div class="w-1/2 h-1/2 ">My Name Is Fadwa</div>
  <br/>
  <div class="w-1/2 h-1/2 ">{{name}}</div>
  <br/>
  <div class="w-1/2 h-1/2 " v-text="name"></div>
</template>
<script>
export default {
  namw: "App",
  data() {
    return {
      name: "Fadwa Ali",
    };
  }
}
</script>




