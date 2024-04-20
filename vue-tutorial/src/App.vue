<script>//this begins the script section. 

// This is the default export
export default {

  data() //data function
  {
    return {
      message: "hello world",
      count: 12
    }
  },


  //User defined function (method)

  methods: {
    countUp() {
      this.count++ //This will increment the count property.
    },

    resetCount() {
      this.count = 0
    }
  }
}


</script>

<style scoped>
/* Add styles here */
button {
  margin: 5px;
  /* Add some margin between buttons */
}
</style>

<template>
  <h1>{{ message.split("").join("") }}</h1>
  <!-- we use the double curley brackets to get the data -->
  <h2>count is {{ count }}</h2>
  <button @click="countUp">Count Up</button>
  <button @click="resetCount">Reset</button>
</template>