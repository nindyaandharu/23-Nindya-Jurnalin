<template>
<v-app>
  <v-card color="#66806A">
    <v-card-title class="text-center justify-center py-6">
      <h1 class="font-weight-bold text-h2 white--text">
        JURNALIN
      </h1>
    </v-card-title>

    <v-tabs
      v-model="tab"
      background-color="transparent"
      color="white"
      grow
    >
      <v-tab
        v-for="item in items"
        :key="item"
      >
        {{ item }}
      </v-tab>
    </v-tabs>

    <v-tabs-items v-model="tab">
      <v-tab-item
        v-for="item in items"
        :key="item"
      >
        <v-card
          color="basil"
          flat
        >
          
        </v-card>
      </v-tab-item>
    </v-tabs-items>
  </v-card>

  <!-- Sizes your content based upon application components -->
  <v-main>

    <!-- Provides the application the proper gutter -->
    
      <v-img src="./assets/Rectangle 7.png" width="900" height="450" class="mt-10">
      <v-card-text> 
        <H3>HAI, NINDYA! SAVE YOUR MEMORIES FOR TODAY!</H3>
      </v-card-text>
      </v-img>
      <v-card-text class="text-choose mt-5" align="center">choose according to your needs</v-card-text>

    <v-container class="mt-5">
    <v-row>
      <v-col
        cols="12"
        md="6"
      >
      <v-img src="./assets/Ellipse 2.png" width="308" height="302"></v-img>
      </v-col>
      <v-col
        cols="12"
        md="6"
      >
      <v-card-text class="text-diary" align="left"> 
        DIARY
      </v-card-text>
      </v-col>
      <v-col
        cols="12"
        md="6"
      >
        <v-img src="./assets/Ellipse 4.png" width="308" height="302"></v-img>
      </v-col>
      <v-col
        cols="12"
        md="6"
      >
        <v-textarea
          outlined
          name="input-7-4"
          label="Outlined textarea"
          value="The Woodman set to work at once, and so sharp was his axe that the tree was soon chopped nearly through."
        ></v-textarea>
      </v-col>
      <v-col
        cols="12"
        md="6"
      >
        <v-img src="./assets/Ellipse 5.png" width="308" height="302"></v-img>
      </v-col>
      <v-col
        cols="12"
        md="6"
      >
        <v-textarea
          outlined
          name="input-7-4"
          label="Outlined textarea"
          value="The Woodman set to work at once, and so sharp was his axe that the tree was soon chopped nearly through."
        ></v-textarea>
      </v-col>
    </v-row>
  </v-container>
      <!-- If using vue-router -->
      <router-view></router-view>
    
  </v-main>

  <v-footer app>
    footer
    <!-- -->
  </v-footer>
</v-app>
</template>

<script>
export default {
  data: () => {
    return {
        tab: null,
        items: [
          'HOME', 'DIARY', 'CALENDER MOOD', 'TO DO','ABOUT US'
        ],
      }
  },
};
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Asap:ital,wght@1,500&display=swap');
.text-choose{
  font-family: 'Asap';
  font-size: 24px;
}
@import url('https://fonts.googleapis.com/css2?family=Asap&display=swap');
.text-diary{
  font-family: 'Asap';
  font-size: 36px;
}
</style>