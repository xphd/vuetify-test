<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <v-app id="inspire">
      <v-container fluid grid-list-xl>
        <v-layout wrap align-center>
          <v-flex xs12 sm6 d-flex>
            <v-select :items="items" label="Standard"></v-select>
          </v-flex>

          <v-flex xs12 sm6 d-flex>
            <v-select :items="items" box label="Box style"></v-select>
          </v-flex>

          <v-flex xs12 sm6 d-flex>
            <v-select :items="items" label="Outline style" outline></v-select>
          </v-flex>

          <v-flex xs12 sm6 d-flex>
            <v-select :items="items" label="Solo field" solo></v-select>
          </v-flex>
        </v-layout>
      </v-container>
    </v-app>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String
  },
  data() {
    return {
      items: ["Foo", "Bar", "Fizz", "Buzz"]
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
/* h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
} */
</style>
