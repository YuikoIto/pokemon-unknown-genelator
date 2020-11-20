<template>
  <v-container>
    <v-row>
      <v-col cols="12" sm="12" md="6">
        <v-text-field
          @change="changeText"
          label="原文"
          placeholder="アンノーン文字にしたいものを入力してください"></v-text-field>

      </v-col>
    </v-row>
    <v-row>
      <v-col cols="12" sm="12" md="6">
        <p>アンノーン文字</p>
        <div class = "unknownStyle">
          {{ this.text }}
        </div>
      </v-col>
    </v-row>
  </v-container>
</template>
<style scoped>
.unknownStyle {
  font-family: "Unknown Gothic VB", arial, serif;
}
</style>

<script>
  export default {
    name: 'HelloWorld',

    data: () => ({
      text: ''
    }),
    methods: {
      changeText(e) {
        this.text = e;
      }
    }
  }
</script>
