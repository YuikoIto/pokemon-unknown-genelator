<template>
  <v-container>
    <v-card
     class="mx-auto"
     >
     <v-card-text>
       <h2>アンノーン文字変換</h2>
       <div>これは簡単にアンノーン文字に変換できるサービスです。アンノーン文字で書いたものを共有しよう</div>
     </v-card-text>
    </v-card>
    <v-row>
      <v-col cols="12" sm="12" md="6">
        <v-text-field
          v-model="text"
          label="原文"
          placeholder="アンノーン文字にしたいものを入力してください"
        ></v-text-field>
      </v-col>
    </v-row>
    <v-row>
      <v-col cols="12" sm="12" md="6">
        <p>アンノーン文字</p>
        <div class = "unknownStyle">
          {{ text }}
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
    }
  }
</script>
